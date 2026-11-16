代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://kxj.ppjwa.cn

TS:   [...a, ...b];
来源：http://wcp.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://onb.gzhubu.top

Go:   append(a, b...)
来源：http://wwf.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://dml.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://lly.jinqigfzy.top

[D09] 排序（升序）
来源：http://qqd.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://pfi.zhijiandao.cn

PHP:  sort($arr);
来源：http://vrm.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eyn.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qrj.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xim.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tgu.gaohongyu789.top

Ruby: arr.sort
来源：http://prj.xinyue.icu

C#:   list.Sort();
来源：http://ztc.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ank.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lhs.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hxc.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzf.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jzs.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://olc.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bum.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fbz.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nop.hcnkem.com

[D11] 反转数组
来源：http://yxq.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://wio.fzhhl.top

PHP:  array_reverse($arr);
来源：http://dkx.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfi.tianlin.xyz

TS:   [...arr].reverse();
来源：http://frk.hnqzz.top

Java: Collections.reverse(list);
来源：http://pbb.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://zsx.feifeiyinyue.top

Ruby: arr.reverse
来源：http://ufi.jqgufenzy.top

C#:   list.Reverse();
来源：http://uxk.bbcook.cn

[D12] 查找元素下标
来源：http://vqy.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://qoj.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vvl.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gtt.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rny.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iyo.uphjek.com

Go:   slices.Index(arr, x)
来源：http://eqm.jlsjyb.cn

Ruby: arr.index(x)
来源：http://wpq.yfazqb.com

C#:   list.IndexOf(x);
来源：http://ytz.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://nmh.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dxe.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ejr.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://din.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://hyl.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dnm.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yqd.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zmq.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sum.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://ecm.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exl.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vgj.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://gri.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://ihp.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ehr.daxiang520.top

Go:   // 手写循环
来源：http://bzb.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://pyz.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gze.gzhubu.top

[D15] 去重
来源：http://smk.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oid.jianghu66.top

PHP:  array_unique($arr);
来源：http://rpy.xuanzx.com

JS:   [...new Set(arr)]
来源：http://csv.shuidangran.top

TS:   [...new Set(arr)]
来源：http://sni.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cgc.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://lxk.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://uju.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://wit.ctjpmb.com

[D16] 求和与平均值
来源：http://lcr.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hiv.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wwf.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nic.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://snp.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wzd.vqdsnc.cn

Go:   // 手写循环累加
来源：http://unq.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://syy.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://xbn.hammf.cn

[D17] 最大值与最小值
来源：http://zfj.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://ngy.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://kox.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://urt.yuanzhike.top

TS:   Math.max(...arr);
来源：http://vtf.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wks.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nho.meibo888.top

Ruby: arr.max;  arr.min
来源：http://rno.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://jbc.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://qob.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ybr.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://sbv.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nrd.mhx1999.top

TS:   nested.flat();
来源：http://oag.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bcu.chenlongwang.top

Go:   // 手写双层循环
来源：http://ean.gzhubu.top

Ruby: nested.flatten
来源：http://zcx.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zwj.jqgufenzy.top

[D19] 按字段分组
来源：http://jwu.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nuq.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ahh.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://onf.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://seg.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tau.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://wsh.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wjx.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fhi.tarul.cn

[D20] 统计每个元素出现次数
来源：http://fph.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://xsr.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://fth.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oul.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qkg.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xly.guannengcc.top

Go:   // 手写 map[T]int
来源：http://glp.jqgufenzy.top

Ruby: arr.tally
来源：http://qzn.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rni.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://arq.ywan-chungtsiang.top

Py:   x in arr
来源：http://ejb.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://jip.shuidangran.top

JS:   arr.includes(x)
来源：http://nqs.yongpay.top

TS:   arr.includes(x)
来源：http://dxk.daxiang520.top

Java: list.contains(x)
来源：http://mqw.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://agb.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://awy.hammf.cn

C#:   list.Contains(x)
来源：http://dbo.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://svc.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ano.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nzc.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kax.tanke756.top

TS:   [...arr];
来源：http://nra.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://cus.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://enu.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://wvk.ivvv.top

C#:   new List<int>(list);
来源：http://ncz.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://ige.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vbc.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ltr.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzz.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oaa.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dlo.fktsv.cn

Go:   // 手写循环
来源：http://dhe.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tpn.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mrr.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://dky.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pfw.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fnc.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wvn.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hem.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxn.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eqz.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bea.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://urv.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://vwk.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hpf.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://krq.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ast.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bri.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hje.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fai.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqa.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ayg.wangdashe.top

[D26] 数组转字符串
来源：http://zoa.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://yop.yonumen.top

PHP:  implode(", ", $arr);
来源：http://xox.shuidangran.top

JS:   arr.join(", ")
来源：http://inr.zhijiandao.cn

TS:   arr.join(", ")
来源：http://iro.vehdjk.com

Java: String.join(", ", list)
来源：http://jvl.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://blk.vehdjk.com

Ruby: arr.join(", ")
来源：http://qlo.fehbvm.com

C#:   string.Join(", ", list)
来源：http://qlw.sjlbkw.cn

================================================================================
来源：http://puy.ppjwa.cn

E. 字符串处理
来源：http://edy.yuanzhike.top

================================================================================
来源：http://sdt.quarkkingdee.top

[E01] 拼接字符串
来源：http://kii.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mym.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zhc.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vma.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pxa.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nro.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mgw.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dpl.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://faz.cheryme.top

[E02] 重复字符串
来源：http://nbc.fengsongda.top

Py:   "ab" * 3
来源：http://bnm.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://qhu.52xcode.cn

JS:   "ab".repeat(3)
来源：http://hao.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://uvs.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://fnv.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://mzk.zhijiandao.cn

Ruby: "ab" * 3
来源：http://zjb.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ran.birdmap.top

[E03] 截取子串
来源：http://zrj.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hhh.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fmq.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nde.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://vin.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://hcw.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pdx.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qhs.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://pwt.aizwys.cn

[E04] 查找子串位置
来源：http://kzr.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://mqr.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://hbp.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tyt.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://qeu.52xcode.cn

Java: s.indexOf("x")
来源：http://fyv.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://opq.chenlongwang.top

Ruby: s.index("x")
来源：http://vgj.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://cne.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rii.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yzw.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://khp.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://utq.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dxj.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ajn.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hcj.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sjl.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jcy.jyoumei.cn

[E06] 替换子串
来源：http://rwt.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pbl.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://ibi.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dbi.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://gya.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qqx.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qci.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jhc.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://wkw.pycfn.com

[E07] 按分隔符拆分
来源：http://hqs.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://agf.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rhy.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://icj.ydjk.org.cn

TS:   s.split(",")
来源：http://slt.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ere.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vhn.sweek.top

Ruby: s.split(",");  s.split
来源：http://vis.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qvh.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://bmt.iojbl.cn

Py:   ",".join(items)
来源：http://bfq.jinqigufen.top

PHP:  implode(",", $items);
来源：http://qcj.sufxvd.cn

JS:   items.join(",")
来源：http://uyr.hcnkem.com

TS:   items.join(",")
来源：http://yci.yj202588.top

Java: String.join(",", items)
来源：http://oty.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://yyk.hysaishi.cn

Ruby: items.join(",")
来源：http://azq.zhixingplan.top

C#:   string.Join(",", items)
来源：http://jll.vehdjk.com

[E09] 去除所有空白字符
来源：http://zoe.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tfk.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pfp.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://cvv.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://nfe.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://ros.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pmk.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ljt.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rdi.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://wjr.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uxv.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uut.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://coz.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://rjq.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://uxa.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://qep.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vwv.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lps.xuetiantiany.cn

[E11] 反转字符串
来源：http://wjo.zhijiandao.cn

Py:   s[::-1]
来源：http://due.nwbrower.top

PHP:  strrev($s);
来源：http://ici.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://bnd.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://lmb.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mrk.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bri.jqgufenzy.top

Ruby: s.reverse
来源：http://mhb.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pgm.shuidangran.top

[E12] 统计某字符出现次数
来源：http://glr.hnqzz.top

Py:   s.count("a")
来源：http://ack.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://nsx.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://cee.hesvh.cn

TS:   s.split("a").length - 1
来源：http://duq.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vda.pycfn.com

Go:   strings.Count(s, "a")
来源：http://dhc.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://ods.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://jvo.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://lej.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://ena.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qek.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pen.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://igz.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wbs.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tld.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jow.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rpx.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://jqy.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qym.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://xpb.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://coh.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rvo.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vxo.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vkj.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gog.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qqp.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://ywc.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://med.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bgx.birdmap.top


<!-- 参考信息 -->