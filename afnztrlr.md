代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ugw.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iwz.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ici.nanxinkj.top

[D06] 数组长度
来源：http://bzj.snrcjt.cn

Py:   len(arr)
来源：http://wcd.yongpay.top

PHP:  count($arr);
来源：http://laz.xziqi.cn

JS:   arr.length
来源：http://bir.feifeiyinyue.top

TS:   arr.length
来源：http://xdc.sxryk.cn

Java: list.size();
来源：http://wqm.sweek.top

Go:   len(arr)
来源：http://zwy.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://wes.sjlbkw.cn

C#:   list.Count;
来源：http://vhv.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://kho.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ayy.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fhd.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://jua.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://bie.aizwys.cn

Java: list.subList(1, 4);
来源：http://mji.ivvv.top

Go:   arr[1:4]
来源：http://sho.sufxvd.cn

Ruby: arr[1, 3]
来源：http://bnv.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://upl.zhongyouzk.top

[D08] 合并两个数组
来源：http://xmh.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://mht.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://pqn.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ggd.xinyue.icu

TS:   [...a, ...b];
来源：http://our.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kvl.vqdsnc.cn

Go:   append(a, b...)
来源：http://let.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://mwb.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://bdp.hesvh.cn

[D09] 排序（升序）
来源：http://fbn.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://nsw.bjfxy.top

PHP:  sort($arr);
来源：http://vhn.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yor.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ywf.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qcv.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dmr.fehbvm.com

Ruby: arr.sort
来源：http://vsw.pengpengdd.cyou

C#:   list.Sort();
来源：http://ukc.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eaz.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zja.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://adm.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tpo.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xpo.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://emw.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://odm.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ihz.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iip.c1oappe.top

[D11] 反转数组
来源：http://job.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://nxk.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://zbe.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://igt.aizwys.cn

TS:   [...arr].reverse();
来源：http://gsb.fehbvm.com

Java: Collections.reverse(list);
来源：http://mgt.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://xct.hnxiangtu.top

Ruby: arr.reverse
来源：http://wuj.mhx1999.top

C#:   list.Reverse();
来源：http://ucy.sysykeji.top

[D12] 查找元素下标
来源：http://xnx.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://cam.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oks.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vup.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kpk.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hgw.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://ade.meibo888.top

Ruby: arr.index(x)
来源：http://uwj.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://vbz.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://vmy.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mtt.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wpv.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://gfs.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://ghe.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rav.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tcb.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://azc.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://msk.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://rlp.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xwq.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dbo.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://fzu.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://ple.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://foo.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://nbn.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fuo.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hfd.chenjidiqi.icu

[D15] 去重
来源：http://rns.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nnm.wangdashe.top

PHP:  array_unique($arr);
来源：http://usx.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://juj.hammf.cn

TS:   [...new Set(arr)]
来源：http://mgu.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iec.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://ffz.yj20258888.top

Ruby: arr.uniq
来源：http://dsw.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://mbk.zhoulong.xyz

[D16] 求和与平均值
来源：http://yym.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://neb.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uch.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fzg.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://grc.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uwv.xziqi.cn

Go:   // 手写循环累加
来源：http://yhi.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aid.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://qvm.yongpay.top

[D17] 最大值与最小值
来源：http://cqc.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://ouj.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://aop.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ibx.ybcxt.top

TS:   Math.max(...arr);
来源：http://xvo.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fdt.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jum.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://vxn.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://zbu.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://lui.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pxr.yongpay.top

PHP:  array_merge(...$nested);
来源：http://pqm.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mdq.jinqigfzy.top

TS:   nested.flat();
来源：http://vil.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tmx.aibaodan.cn

Go:   // 手写双层循环
来源：http://fhx.tianlin.xyz

Ruby: nested.flatten
来源：http://xbv.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vbq.quarkkingdee.top

[D19] 按字段分组
来源：http://aab.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yij.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zsk.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vyn.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iqu.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wzz.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://rjr.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hhi.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pio.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://izo.aizwys.cn

Py:   Counter(arr)
来源：http://zch.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://wua.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://axn.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xne.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dsd.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://lsj.ybcxt.top

Ruby: arr.tally
来源：http://haw.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gkk.daria6918.cn

[D21] 判断是否包含某元素
来源：http://gwx.zhijiandao.cn

Py:   x in arr
来源：http://owf.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://uir.haohaochexian.top

JS:   arr.includes(x)
来源：http://uhg.hnxiangtu.top

TS:   arr.includes(x)
来源：http://qrl.jlsjyb.cn

Java: list.contains(x)
来源：http://obr.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://qdk.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://dzo.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://dfk.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://peq.tarul.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iaf.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lmo.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qps.nwbrower.top

TS:   [...arr];
来源：http://qqs.cashguo.top

Java: new ArrayList<>(list);
来源：http://csi.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://wym.bjfxy.top

Ruby: arr.dup;  arr.clone
来源：http://rud.redwolf501.top

C#:   new List<int>(list);
来源：http://qew.shuidangran.top

[D23] reduce 累积计算
来源：http://vck.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ybp.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gss.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gcv.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jyo.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://duk.epnwcf.com

Go:   // 手写循环
来源：http://phx.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jej.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vpy.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://cdw.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dxb.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pac.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skm.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dph.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zkm.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vla.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mma.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qtf.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://vwa.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tzu.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lhe.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yyv.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://koi.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mlc.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vyp.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eaj.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ypy.birdmap.top

[D26] 数组转字符串
来源：http://ghl.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://tgr.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://eqn.chenlongwang.top

JS:   arr.join(", ")
来源：http://tgi.0kj1m.cn

TS:   arr.join(", ")
来源：http://oek.gogol.net.cn

Java: String.join(", ", list)
来源：http://xxr.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://vif.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://ush.smart0.xyz

C#:   string.Join(", ", list)
来源：http://ctf.tianlin.xyz

================================================================================
来源：http://qif.aibaodan.cn

E. 字符串处理
来源：http://kxq.fehbvm.com

================================================================================
来源：http://gfb.yj202588.top

[E01] 拼接字符串
来源：http://uis.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dxl.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bnn.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mhc.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zmd.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nmx.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://efg.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vij.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://huk.quarkkingdee.top

[E02] 重复字符串
来源：http://kri.jqgfzy.top

Py:   "ab" * 3
来源：http://aod.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://noo.hammf.cn

JS:   "ab".repeat(3)
来源：http://hjf.ybcxt.top

TS:   "ab".repeat(3)
来源：http://ivm.shuidangran.top

Java: "ab".repeat(3)
来源：http://lyz.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://qmh.xinyue.icu

Ruby: "ab" * 3
来源：http://czu.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://csk.cdnleiting.top

[E03] 截取子串
来源：http://squ.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qau.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqd.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rgc.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://iaf.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://msn.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vcv.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rno.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://wxl.jinqigufen.top

[E04] 查找子串位置
来源：http://ewv.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://ksv.shuidangran.top

PHP:  strpos($s, "x");
来源：http://xbh.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zgz.yfazqb.com

TS:   s.indexOf("x")
来源：http://shd.ivvv.top

Java: s.indexOf("x")
来源：http://jfo.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://ikq.vqdsnc.cn

Ruby: s.index("x")
来源：http://iax.redwolf501.top

C#:   s.IndexOf("x")
来源：http://ujn.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://nik.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wuk.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kis.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djz.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yxz.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtk.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qbo.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gtf.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gpb.xuanzx.com

[E06] 替换子串
来源：http://msb.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://evy.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://mqd.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jyg.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://shl.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wwb.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vtp.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pxk.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://jjd.epnwcf.com

[E07] 按分隔符拆分
来源：http://qnu.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rtd.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vek.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://yql.jlsjyb.cn

TS:   s.split(",")
来源：http://zcu.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dgd.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vei.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://tbi.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bmz.daxiang520.top

[E08] 数组按分隔符合并
来源：http://sms.yueranfly.top

Py:   ",".join(items)
来源：http://gjr.aizwys.cn

PHP:  implode(",", $items);
来源：http://tcj.tanke756.top

JS:   items.join(",")
来源：http://cbq.daxiang520.top

TS:   items.join(",")
来源：http://ghn.chenjidiqi.icu

Java: String.join(",", items)
来源：http://scp.cheryme.top

Go:   strings.Join(items, ",")
来源：http://zxu.hnqzz.top

Ruby: items.join(",")
来源：http://yim.meibo888.top

C#:   string.Join(",", items)
来源：http://lho.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://isj.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vly.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vcx.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://gcv.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://fwh.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://fiw.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://faq.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://krn.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://emv.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://fjs.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://syf.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wes.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://nqv.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://sab.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://fxz.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ocp.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://emt.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cdr.kuanghao11.cn

[E11] 反转字符串
来源：http://cmt.cucudq.cn

Py:   s[::-1]
来源：http://ccq.jinqigufen.top

PHP:  strrev($s);
来源：http://fxc.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://tty.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://opg.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://ycx.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://eaw.jinqigfzy.top

Ruby: s.reverse
来源：http://lrf.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hsm.tanke756.top

[E12] 统计某字符出现次数
来源：http://mag.sufxvd.cn

Py:   s.count("a")
来源：http://hzc.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://nsh.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://sqq.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://qip.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cnn.ivvv.top


<!-- 参考信息 -->