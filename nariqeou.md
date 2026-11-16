代发 wailian999

[D07] 切片 / 取子数组
来源：http://ttk.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wxk.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://nga.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://grd.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://eii.zhengqikj.top

Java: list.subList(1, 4);
来源：http://tfu.tarul.cn

Go:   arr[1:4]
来源：http://qns.hfpthk.cn

Ruby: arr[1, 3]
来源：http://qge.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://vqw.yuanzhike.top

[D08] 合并两个数组
来源：http://svr.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://ena.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://sth.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nxo.yj20258888.top

TS:   [...a, ...b];
来源：http://wqm.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jfr.redwolf501.top

Go:   append(a, b...)
来源：http://haf.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://mwt.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://fsa.chenzaomai.com

[D09] 排序（升序）
来源：http://baf.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://gtf.wangshuangyany.cn

PHP:  sort($arr);
来源：http://ikc.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rim.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gzv.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ifx.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hio.yfazqb.com

Ruby: arr.sort
来源：http://gnn.yvedp.cn

C#:   list.Sort();
来源：http://whm.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pwa.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ege.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vbv.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ccs.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lux.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eye.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://myi.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bys.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://whu.pengpengdd.cyou

[D11] 反转数组
来源：http://fuo.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://hfi.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://vnr.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iir.iojbl.cn

TS:   [...arr].reverse();
来源：http://aeh.cheryme.top

Java: Collections.reverse(list);
来源：http://hxm.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://jbx.quarkkingdee.top

Ruby: arr.reverse
来源：http://csx.zdqjudy.top

C#:   list.Reverse();
来源：http://eay.bbcook.cn

[D12] 查找元素下标
来源：http://lax.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://nxn.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bhs.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dvi.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrr.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://miy.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://zuh.0kj1m.cn

Ruby: arr.index(x)
来源：http://tvi.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://lxu.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://wem.sweek.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fta.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iui.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://iqq.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://qqy.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zzv.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://igt.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://ldg.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nmh.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://mnm.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vsn.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nib.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://vjb.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://wci.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oem.hysaishi.cn

Go:   // 手写循环
来源：http://xhh.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://nfw.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wmq.ppjwa.cn

[D15] 去重
来源：http://xas.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nht.pycfn.com

PHP:  array_unique($arr);
来源：http://gpn.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://lra.pycfn.com

TS:   [...new Set(arr)]
来源：http://ijv.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cuf.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hzk.nanxuanxn.top

Ruby: arr.uniq
来源：http://emu.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://kwy.ctjpmb.com

[D16] 求和与平均值
来源：http://wcn.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xvg.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pbo.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jgp.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpz.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yzw.yonumen.top

Go:   // 手写循环累加
来源：http://nnf.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rro.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://yxc.gogol.net.cn

[D17] 最大值与最小值
来源：http://rdp.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://kmb.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://hmj.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cum.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://eda.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tqv.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jrt.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://zxd.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://nqt.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://eoo.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://shm.yonumen.top

PHP:  array_merge(...$nested);
来源：http://hdk.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://azg.ybcxt.top

TS:   nested.flat();
来源：http://iwy.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://thk.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://shb.pycfn.com

Ruby: nested.flatten
来源：http://bxc.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ufa.fktsv.cn

[D19] 按字段分组
来源：http://kgg.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nmm.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rdr.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ait.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ooc.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://por.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://lci.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uxy.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wuk.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://lin.feifeiyinyue.top

Py:   Counter(arr)
来源：http://qqo.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://vof.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gxw.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ryr.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggd.yonumen.top

Go:   // 手写 map[T]int
来源：http://ryq.shuidangran.top

Ruby: arr.tally
来源：http://qhn.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://umf.nwbrower.top

[D21] 判断是否包含某元素
来源：http://miu.redwolf501.top

Py:   x in arr
来源：http://apa.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://mvk.cdnleiting.top

JS:   arr.includes(x)
来源：http://zxo.dashuyun.cn

TS:   arr.includes(x)
来源：http://nlj.fanxiaobao.xyz

Java: list.contains(x)
来源：http://wua.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://thi.bbcook.cn

Ruby: arr.include?(x)
来源：http://eih.cdnleiting.top

C#:   list.Contains(x)
来源：http://uwb.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://dml.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://boa.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uta.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nyk.birdmap.top

TS:   [...arr];
来源：http://hcu.xziqi.cn

Java: new ArrayList<>(list);
来源：http://chc.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://ash.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://arr.havefunace.top

C#:   new List<int>(list);
来源：http://iah.xinyue.icu

[D23] reduce 累积计算
来源：http://tco.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wro.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uvo.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wie.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pvj.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://rbl.ctjpmb.com

Go:   // 手写循环
来源：http://wkw.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cpw.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qgk.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://lqm.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://chc.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rxn.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rmx.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fnc.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gzu.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dua.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yrl.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lks.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://oqy.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sjh.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pac.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kkj.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pyw.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kdh.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zgi.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://evt.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zkj.epnwcf.com

[D26] 数组转字符串
来源：http://smf.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://fav.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://hdu.ivvv.top

JS:   arr.join(", ")
来源：http://pqf.uphjek.com

TS:   arr.join(", ")
来源：http://zir.pycfn.com

Java: String.join(", ", list)
来源：http://man.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://uen.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://cow.andypj.xyz

C#:   string.Join(", ", list)
来源：http://zbf.redwolf501.top

================================================================================
来源：http://dfd.bbcook.cn

E. 字符串处理
来源：http://ufz.meibo888.top

================================================================================
来源：http://rwi.daxiang520.top

[E01] 拼接字符串
来源：http://nya.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uck.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lrk.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wmw.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ebp.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rau.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wvg.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uqo.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://too.hywenlv.cn

[E02] 重复字符串
来源：http://cfw.zhijiandao.cn

Py:   "ab" * 3
来源：http://wgj.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://mhl.yj20258.top

JS:   "ab".repeat(3)
来源：http://ozu.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://biq.aibaodan.cn

Java: "ab".repeat(3)
来源：http://wxi.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://bfi.wangdashe.top

Ruby: "ab" * 3
来源：http://kjm.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://orc.shuidangran.top

[E03] 截取子串
来源：http://mkl.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qba.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hpl.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mev.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://tkh.gogol.net.cn

Java: s.substring(1, 4)
来源：http://hcm.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rtq.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ven.sweek.top

C#:   s.Substring(1, 3)
来源：http://ypn.daria6918.cn

[E04] 查找子串位置
来源：http://oya.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://htk.pycfn.com

PHP:  strpos($s, "x");
来源：http://gxb.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lzi.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://gvy.yuxming.cn

Java: s.indexOf("x")
来源：http://oty.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://alq.hammf.cn

Ruby: s.index("x")
来源：http://qky.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://fqs.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://kyb.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hre.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://buc.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhd.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hzo.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sgg.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mgm.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pcu.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oyo.shuidangran.top

[E06] 替换子串
来源：http://fgi.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dkq.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://uwd.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://poa.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://jhs.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rlb.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://maw.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nqw.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://xwz.hfpthk.cn

[E07] 按分隔符拆分
来源：http://cqu.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vfu.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gml.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dwc.shuidangran.top

TS:   s.split(",")
来源：http://kde.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://czo.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cvy.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://exi.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zjj.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://cvw.kuanghao11.cn

Py:   ",".join(items)
来源：http://xbh.yj20258.top

PHP:  implode(",", $items);
来源：http://kqt.fehbvm.com

JS:   items.join(",")
来源：http://mem.jinqigufen.top

TS:   items.join(",")
来源：http://yuj.xuetiantiany.cn

Java: String.join(",", items)
来源：http://hdq.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://xgy.zhijiandao.cn

Ruby: items.join(",")
来源：http://iaj.sxryk.cn

C#:   string.Join(",", items)
来源：http://vlf.jyoumei.cn

[E09] 去除所有空白字符
来源：http://wjl.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://meq.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wfx.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://bom.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://grd.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://jjt.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ghs.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://pzo.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kzw.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://rxy.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fwu.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nga.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://tit.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://zvg.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://tjr.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xht.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sgb.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xzr.jinghuilouyu.cn

[E11] 反转字符串
来源：http://tjy.dashuyun.cn

Py:   s[::-1]
来源：http://dus.tianlin.xyz

PHP:  strrev($s);
来源：http://cur.cheryme.top

JS:   [...s].reverse().join("")
来源：http://paz.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://iwu.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ots.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://std.shzxlz.cn

Ruby: s.reverse
来源：http://dfl.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uvo.yueranfly.top

[E12] 统计某字符出现次数
来源：http://vna.shangyingyoupin.top

Py:   s.count("a")
来源：http://kgk.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://goz.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://tza.yongpay.top

TS:   s.split("a").length - 1
来源：http://lok.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://svv.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://adt.pengpengdd.cyou

Ruby: s.count("a")
来源：http://atu.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://hur.wangdashe.top

[E13] 逐字符遍历
来源：http://kzq.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://bzg.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fhy.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwm.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ipn.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pan.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qaw.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zny.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nld.yj202588.top


<!-- 参考信息 -->