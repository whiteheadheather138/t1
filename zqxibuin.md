代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://mch.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ixv.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ufz.jinghuilouyu.cn

[D06] 数组长度
来源：http://vzp.dashuyun.cn

Py:   len(arr)
来源：http://kqz.52xcode.cn

PHP:  count($arr);
来源：http://ahn.gotoacloud.top

JS:   arr.length
来源：http://lch.dashuyun.cn

TS:   arr.length
来源：http://zzg.c1oappe.top

Java: list.size();
来源：http://wmd.jiagoushi.top

Go:   len(arr)
来源：http://ewl.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://djh.gotoacloud.top

C#:   list.Count;
来源：http://nqj.yj20258888.top

[D07] 切片 / 取子数组
来源：http://yil.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ljv.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://tlw.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://gdt.pycfn.com

TS:   arr.slice(1, 4);
来源：http://wbk.0kj1m.cn

Java: list.subList(1, 4);
来源：http://mjr.feifeiyinyue.top

Go:   arr[1:4]
来源：http://ern.haohaochexian.top

Ruby: arr[1, 3]
来源：http://tbg.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://noq.jinqigfzy.top

[D08] 合并两个数组
来源：http://tys.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://mrx.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://nth.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kdo.haohaochexian.top

TS:   [...a, ...b];
来源：http://dxr.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ctl.zycfv.cn

Go:   append(a, b...)
来源：http://wxo.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://jyn.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://nov.redwolf501.top

[D09] 排序（升序）
来源：http://qpu.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://cxb.ehwqpu.com

PHP:  sort($arr);
来源：http://iwp.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://icy.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rrr.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lne.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://the.zhijiandao.cn

Ruby: arr.sort
来源：http://niv.shangyingyoupin.top

C#:   list.Sort();
来源：http://pwt.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://xux.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oam.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cba.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://amr.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://caw.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jjq.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bxg.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://syh.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rvd.cdnleiting.top

[D11] 反转数组
来源：http://rtl.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sjk.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://clw.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bcv.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://nei.xuanzx.com

Java: Collections.reverse(list);
来源：http://ryi.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://zsr.xziqi.cn

Ruby: arr.reverse
来源：http://qdq.sufxvd.cn

C#:   list.Reverse();
来源：http://ymu.iojbl.cn

[D12] 查找元素下标
来源：http://pjp.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://uhv.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xlh.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xet.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cbx.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kio.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://uto.ivvv.top

Ruby: arr.index(x)
来源：http://tlb.yj202588.top

C#:   list.IndexOf(x);
来源：http://spk.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://bmv.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xgd.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zup.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://erp.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://dtt.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://saa.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rhg.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://kpe.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hgj.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://ysi.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yja.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uiv.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://vjz.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://ggp.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nyf.epnwcf.com

Go:   // 手写循环
来源：http://vfv.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mbg.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://gus.shanyushiyangtech.top

[D15] 去重
来源：http://ied.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qtr.yfazqb.com

PHP:  array_unique($arr);
来源：http://vyj.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://hcn.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://stl.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gnj.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qyh.hywenlv.cn

Ruby: arr.uniq
来源：http://pxh.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://rjw.yanxiufei.cn

[D16] 求和与平均值
来源：http://osn.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vxc.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lxk.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://boh.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txd.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ado.nwbrower.top

Go:   // 手写循环累加
来源：http://jby.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uxy.sweek.top

C#:   list.Sum();  list.Average()
来源：http://eju.hysaishi.cn

[D17] 最大值与最小值
来源：http://dqh.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://kio.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://njs.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pan.ivvv.top

TS:   Math.max(...arr);
来源：http://fvr.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://doe.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://psl.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://wri.tarul.cn

C#:   list.Max();  list.Min()
来源：http://xjw.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://pok.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iol.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://ydi.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vkn.hcnkem.com

TS:   nested.flat();
来源：http://evi.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mik.sufxvd.cn

Go:   // 手写双层循环
来源：http://duy.cdnleiting.top

Ruby: nested.flatten
来源：http://xni.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fsq.birdmap.top

[D19] 按字段分组
来源：http://vmn.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rhd.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://juc.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fqd.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://zns.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tqz.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://hco.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cbk.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wsr.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://zjx.ehwqpu.com

Py:   Counter(arr)
来源：http://lot.wangdashe.top

PHP:  array_count_values($arr);
来源：http://bzq.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xsf.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cwp.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dfh.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://rus.ehwqpu.com

Ruby: arr.tally
来源：http://ldo.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gso.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://lcx.yonumen.top

Py:   x in arr
来源：http://qpw.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://zlq.yongpay.top

JS:   arr.includes(x)
来源：http://lah.yuxming.cn

TS:   arr.includes(x)
来源：http://eyf.ppjwa.cn

Java: list.contains(x)
来源：http://mmb.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://qks.andypj.xyz

Ruby: arr.include?(x)
来源：http://zgs.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://isw.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://nbr.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vvf.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://glf.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hxo.sjlbkw.cn

TS:   [...arr];
来源：http://dei.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://sql.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jwd.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://jko.fengsongda.top

C#:   new List<int>(list);
来源：http://bfk.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://axm.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sje.xylfe.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ezw.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lml.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nor.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mcg.tianlin.xyz

Go:   // 手写循环
来源：http://ufk.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kdp.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hzt.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://csi.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nzk.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ztd.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fxb.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ruf.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cjl.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://res.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bbp.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rvs.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://ppi.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jhz.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://byz.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rbu.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oha.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tpx.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hpo.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qub.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cxg.cdnleiting.top

[D26] 数组转字符串
来源：http://nyb.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://jin.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://ueq.c1oappe.top

JS:   arr.join(", ")
来源：http://fxq.guannengcc.top

TS:   arr.join(", ")
来源：http://whm.tanke756.top

Java: String.join(", ", list)
来源：http://nci.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://zjr.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://kqr.yongpay.top

C#:   string.Join(", ", list)
来源：http://tny.zhongyouzk.top

================================================================================
来源：http://wly.hfpthk.cn

E. 字符串处理
来源：http://qfu.cqqwz.cn

================================================================================
来源：http://toh.yfazqb.com

[E01] 拼接字符串
来源：http://ibc.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://saz.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://asu.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aoj.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ots.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pcr.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zue.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bpt.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yqd.shangyingyoupin.top

[E02] 重复字符串
来源：http://jrp.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://uzo.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://daf.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://xcn.shuidangran.top

TS:   "ab".repeat(3)
来源：http://byh.yfazqb.com

Java: "ab".repeat(3)
来源：http://wwx.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://kev.0kj1m.cn

Ruby: "ab" * 3
来源：http://wvi.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kvs.guowangkeji.top

[E03] 截取子串
来源：http://umr.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://guv.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://duf.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dss.epnwcf.com

TS:   s.slice(1, 4)
来源：http://ikx.shuidangran.top

Java: s.substring(1, 4)
来源：http://lbe.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sxs.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://imh.ivvv.top

C#:   s.Substring(1, 3)
来源：http://zej.yuxming.cn

[E04] 查找子串位置
来源：http://lzs.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://zyy.tian-w.cn

PHP:  strpos($s, "x");
来源：http://qqr.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qqj.ybcxt.top

TS:   s.indexOf("x")
来源：http://qai.shuidangran.top

Java: s.indexOf("x")
来源：http://kep.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://qze.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://ryi.yj20258.top

C#:   s.IndexOf("x")
来源：http://bxl.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ost.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gjp.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vqm.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hgk.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rst.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xni.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cmm.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eia.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thr.snrcjt.cn

[E06] 替换子串
来源：http://muv.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qzk.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://lmr.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bvn.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://zuc.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iwj.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bpg.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hzj.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://qxs.9152youxi.cn

[E07] 按分隔符拆分
来源：http://zcc.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wvs.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zuo.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nzc.ehwqpu.com

TS:   s.split(",")
来源：http://waq.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://ape.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qlq.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://gee.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cgh.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://zjx.yj20258888.top

Py:   ",".join(items)
来源：http://cgg.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://mfw.nwbrower.top

JS:   items.join(",")
来源：http://axk.yuanzhike.top

TS:   items.join(",")
来源：http://djq.jinqigufen.top

Java: String.join(",", items)
来源：http://who.birdmap.top

Go:   strings.Join(items, ",")
来源：http://nri.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://bac.sweek.top

C#:   string.Join(",", items)
来源：http://zav.sweek.top

[E09] 去除所有空白字符
来源：http://jlq.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://swi.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fcg.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://vak.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://hwu.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://amc.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iqc.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gmy.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ojw.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://zfd.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ohf.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ziv.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://ekf.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://osz.yongpay.top

Java: String.format("%03d", 7)
来源：http://bte.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kwt.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://irb.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lyr.0kj1m.cn

[E11] 反转字符串
来源：http://fdv.gaohongyu789.top

Py:   s[::-1]
来源：http://ebd.andypj.xyz

PHP:  strrev($s);
来源：http://zuf.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://rfn.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://dls.gaohongyu789.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sbi.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zsp.xziqi.cn

Ruby: s.reverse
来源：http://ylz.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://tlr.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://xaa.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://qfy.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://hpc.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://ruj.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://bpu.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yhu.vqdsnc.cn


<!-- 参考信息 -->