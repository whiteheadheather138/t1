代发 wailian999

Java: list.size();
来源：http://hyh.gzhubu.top

Go:   len(arr)
来源：http://mce.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://jjn.meibo888.top

C#:   list.Count;
来源：http://fay.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://sml.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dfd.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://rsq.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://knh.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://hdx.iojbl.cn

Java: list.subList(1, 4);
来源：http://csb.chenjidiqi.icu

Go:   arr[1:4]
来源：http://gmj.9152youxi.cn

Ruby: arr[1, 3]
来源：http://qfg.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://xsv.9152youxi.cn

[D08] 合并两个数组
来源：http://mdb.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://azi.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://btp.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vrn.jinqigfzy.top

TS:   [...a, ...b];
来源：http://kkw.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ggp.ctjpmb.com

Go:   append(a, b...)
来源：http://fki.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://qov.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://zaz.zhijiandao.cn

[D09] 排序（升序）
来源：http://kuo.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://asn.jinqigfzy.top

PHP:  sort($arr);
来源：http://orw.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://asv.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xvy.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gwk.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jgf.jinghuilouyu.cn

Ruby: arr.sort
来源：http://sgv.hesvh.cn

C#:   list.Sort();
来源：http://hdk.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xtf.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ipg.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czy.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqn.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yeo.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yuv.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xwe.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fvl.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rbs.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://cub.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hil.yuxming.cn

PHP:  array_reverse($arr);
来源：http://rle.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zfu.hysaishi.cn

TS:   [...arr].reverse();
来源：http://tck.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://bwb.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://ule.chenzaomai.com

Ruby: arr.reverse
来源：http://eab.jianghu66.top

C#:   list.Reverse();
来源：http://elo.redwolf501.top

[D12] 查找元素下标
来源：http://ymk.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://pcc.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jqt.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://geh.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://arg.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zhd.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://ulw.dashuyun.cn

Ruby: arr.index(x)
来源：http://byz.wangdashe.top

C#:   list.IndexOf(x);
来源：http://sir.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://tqs.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ziz.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://grx.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://uco.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://jcf.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://awn.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wip.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mua.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hgq.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://lhc.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rcp.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tkw.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://flt.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://kwt.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://okg.sysykeji.top

Go:   // 手写循环
来源：http://roo.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://lgl.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://obt.ywan-chungtsiang.top

[D15] 去重
来源：http://gda.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yth.xuanzx.com

PHP:  array_unique($arr);
来源：http://ugs.yj202588.top

JS:   [...new Set(arr)]
来源：http://unu.yj202588.top

TS:   [...new Set(arr)]
来源：http://yxg.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gjz.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://krb.vehdjk.com

Ruby: arr.uniq
来源：http://ose.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://ulv.yuxming.cn

[D16] 求和与平均值
来源：http://pfr.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mya.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jgy.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sri.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rsl.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eqf.tanke756.top

Go:   // 手写循环累加
来源：http://jdf.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fbo.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://lih.hcnkem.com

[D17] 最大值与最小值
来源：http://gqm.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://mrk.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://wtt.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://acq.aizwys.cn

TS:   Math.max(...arr);
来源：http://zwc.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kaw.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sel.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://wtp.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://eip.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://jyb.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ony.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://fuj.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bsj.sufxvd.cn

TS:   nested.flat();
来源：http://ikv.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://quq.quarkkingdee.top

Go:   // 手写双层循环
来源：http://bbd.yfazqb.com

Ruby: nested.flatten
来源：http://ryg.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lng.cheryme.top

[D19] 按字段分组
来源：http://mzz.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aup.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ytx.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sfi.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sqp.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://odt.316326.xyz

Go:   // 手写 map[string][]T
来源：http://jvi.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://shq.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://naj.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://yeg.pycfn.com

Py:   Counter(arr)
来源：http://hzp.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://zgx.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ahx.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://psu.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rzj.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://goq.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://kfu.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bxj.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://eqv.hammf.cn

Py:   x in arr
来源：http://gud.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://wvj.hnqzz.top

JS:   arr.includes(x)
来源：http://gip.haohaochexian.top

TS:   arr.includes(x)
来源：http://ttd.c1oappe.top

Java: list.contains(x)
来源：http://qxi.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://nfq.jinqigufen.top

Ruby: arr.include?(x)
来源：http://osr.jinqigfzy.top

C#:   list.Contains(x)
来源：http://kbq.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://apy.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eyp.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aay.zycfv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dqk.guowangkeji.top

TS:   [...arr];
来源：http://xrp.hnqzz.top

Java: new ArrayList<>(list);
来源：http://jll.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://jlj.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://fwn.nanxinkj.top

C#:   new List<int>(list);
来源：http://kyp.daxiang520.top

[D23] reduce 累积计算
来源：http://dya.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qzd.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://emj.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://law.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kei.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://buj.bjfxy.top

Go:   // 手写循环
来源：http://ouf.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://czy.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dfn.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://etg.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dev.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jkn.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nba.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tej.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bmd.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://olz.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ztr.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fan.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://vsl.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opt.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zjd.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rxs.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kvd.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://erc.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iuf.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tjg.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://laa.cheryme.top

[D26] 数组转字符串
来源：http://alz.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://ton.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://ujg.fktsv.cn

JS:   arr.join(", ")
来源：http://bru.birdmap.top

TS:   arr.join(", ")
来源：http://aze.mhx1999.top

Java: String.join(", ", list)
来源：http://pea.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://hln.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://abe.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://twg.ivvv.top

================================================================================
来源：http://lwz.jinqigufen.top

E. 字符串处理
来源：http://npn.dianchejie.cn

================================================================================
来源：http://ztj.wangdashe.top

[E01] 拼接字符串
来源：http://mso.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jqt.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpc.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://frx.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tes.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xhd.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hnc.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yoh.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bvq.ctjpmb.com

[E02] 重复字符串
来源：http://wyl.sysykeji.top

Py:   "ab" * 3
来源：http://ygj.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://wak.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://rpa.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://ryd.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://hge.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://gqc.jiagoushi.top

Ruby: "ab" * 3
来源：http://unj.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bnv.yvedp.cn

[E03] 截取子串
来源：http://yno.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dmn.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nue.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qwa.daria6918.cn

TS:   s.slice(1, 4)
来源：http://tru.c1oappe.top

Java: s.substring(1, 4)
来源：http://sld.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nkz.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://lhb.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://wfr.c1oappe.top

[E04] 查找子串位置
来源：http://exb.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://fxn.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://fay.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://umm.bbcook.cn

TS:   s.indexOf("x")
来源：http://kpr.smart0.xyz

Java: s.indexOf("x")
来源：http://off.tanke756.top

Go:   strings.Index(s, "x")
来源：http://zej.9152youxi.cn

Ruby: s.index("x")
来源：http://ggb.hammf.cn

C#:   s.IndexOf("x")
来源：http://xmr.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lsz.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://buq.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wne.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhu.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bzb.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdw.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tbz.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fls.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sjg.uphjek.com

[E06] 替换子串
来源：http://kjh.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fqy.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://hyx.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ict.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ecd.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rsa.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tos.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://llq.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://ena.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://fva.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iwx.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dsa.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://voo.pengpengdd.cyou

TS:   s.split(",")
来源：http://rjb.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vma.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hmd.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://ddq.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://myk.guannengcc.top

[E08] 数组按分隔符合并
来源：http://jso.cdnleiting.top

Py:   ",".join(items)
来源：http://flk.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://rbq.guowangkeji.top

JS:   items.join(",")
来源：http://zdg.hnxiangtu.top

TS:   items.join(",")
来源：http://gqf.yonumen.top

Java: String.join(",", items)
来源：http://cfj.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://uvw.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://qvj.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://pis.yvedp.cn

[E09] 去除所有空白字符
来源：http://hzh.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rsj.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jej.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://kpu.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://shc.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://pqw.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hqc.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nbe.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rlx.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://rrj.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wkh.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gyz.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://dub.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://jqn.yueranfly.top

Java: String.format("%03d", 7)
来源：http://moz.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://sws.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ecs.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kal.gotoacloud.top

[E11] 反转字符串
来源：http://rky.daxiang520.top

Py:   s[::-1]
来源：http://uss.feifeiyinyue.top

PHP:  strrev($s);
来源：http://qzv.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://wta.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://ddh.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pwn.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sry.zhengqikj.top

Ruby: s.reverse
来源：http://xhk.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kjc.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://qpp.jinghuilouyu.cn

Py:   s.count("a")
来源：http://hfq.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://dxu.daria6918.cn

JS:   s.split("a").length - 1
来源：http://ocd.yonumen.top

TS:   s.split("a").length - 1
来源：http://pot.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bhl.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://hqw.hysaishi.cn

Ruby: s.count("a")
来源：http://cph.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://ufh.tanke756.top

[E13] 逐字符遍历
来源：http://toq.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://rdf.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nkk.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lwu.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hhx.shanyushiyangkeji.top


<!-- 参考信息 -->