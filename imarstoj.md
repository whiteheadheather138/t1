代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ecp.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://blx.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kve.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tgo.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jov.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oho.sweek.top

[D05] 访问与修改元素
来源：http://mpq.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://etd.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pmq.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lcu.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://gyx.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://ylh.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://caz.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ruo.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mfb.hfpthk.cn

[D06] 数组长度
来源：http://ctj.c1oappe.top

Py:   len(arr)
来源：http://ska.jinghuilouyu.cn

PHP:  count($arr);
来源：http://fgr.sweek.top

JS:   arr.length
来源：http://puk.sjlbkw.cn

TS:   arr.length
来源：http://krd.hnxiangtu.top

Java: list.size();
来源：http://qez.hesvh.cn

Go:   len(arr)
来源：http://cim.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://ggu.mhx1999.top

C#:   list.Count;
来源：http://scs.fengsongda.top

[D07] 切片 / 取子数组
来源：http://ibz.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ibz.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://lqd.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://kzq.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://jio.zycfv.cn

Java: list.subList(1, 4);
来源：http://csh.fehbvm.com

Go:   arr[1:4]
来源：http://aim.bbcook.cn

Ruby: arr[1, 3]
来源：http://lyi.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://aha.fzhhl.top

[D08] 合并两个数组
来源：http://qan.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://sgd.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://gaa.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sxz.sysykeji.top

TS:   [...a, ...b];
来源：http://rts.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pgx.yangfankeji.com

Go:   append(a, b...)
来源：http://vnm.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://lql.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://evl.jianghu66.top

[D09] 排序（升序）
来源：http://fij.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://hfs.aizwys.cn

PHP:  sort($arr);
来源：http://odz.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fze.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uuh.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jjo.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vcc.wangdashe.top

Ruby: arr.sort
来源：http://rba.gotoacloud.top

C#:   list.Sort();
来源：http://ofm.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hen.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zjv.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqc.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rnh.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fkw.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jyn.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kgg.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sah.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://znm.smart0.xyz

[D11] 反转数组
来源：http://ahn.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dao.hcnkem.com

PHP:  array_reverse($arr);
来源：http://zxt.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mnk.daxiang520.top

TS:   [...arr].reverse();
来源：http://eyd.ydzc1.top

Java: Collections.reverse(list);
来源：http://ddi.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://ruo.hnqzz.top

Ruby: arr.reverse
来源：http://xou.ivvv.top

C#:   list.Reverse();
来源：http://pmg.iojbl.cn

[D12] 查找元素下标
来源：http://dzl.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://ugm.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zrv.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://drl.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ocn.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vxr.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://ocw.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://pxs.yj20258888.top

C#:   list.IndexOf(x);
来源：http://lma.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://sps.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cro.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jzn.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://mry.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://dky.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://knu.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cjw.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://ekq.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bgz.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://fin.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bjf.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://btt.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://igs.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://adj.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zns.haohaochexian.top

Go:   // 手写循环
来源：http://ais.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ioi.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vro.bjfxy.top

[D15] 去重
来源：http://zua.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sov.9152youxi.cn

PHP:  array_unique($arr);
来源：http://fiv.xziqi.cn

JS:   [...new Set(arr)]
来源：http://mmk.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://ayk.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://apd.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://mwy.hesvh.cn

Ruby: arr.uniq
来源：http://yzn.birdmap.top

C#:   list.Distinct().ToList()
来源：http://ohf.yonumen.top

[D16] 求和与平均值
来源：http://esm.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dsu.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tzm.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxt.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://khp.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wcy.quarkkingdee.top

Go:   // 手写循环累加
来源：http://kxg.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xhf.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://gwv.c1oappe.top

[D17] 最大值与最小值
来源：http://zqy.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://tym.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://qdc.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qik.daria6918.cn

TS:   Math.max(...arr);
来源：http://nws.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://gzn.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jbh.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://stt.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://mvy.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://xud.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fxr.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://pom.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nvo.xuanzx.com

TS:   nested.flat();
来源：http://stl.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yjw.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://etj.snrcjt.cn

Ruby: nested.flatten
来源：http://eoq.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://obi.jyoumei.cn

[D19] 按字段分组
来源：http://tbc.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ece.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kxe.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rbk.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mfl.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tvw.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://kuj.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://odw.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yhh.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://ddr.guowangkeji.top

Py:   Counter(arr)
来源：http://twl.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://xlg.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eqc.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ueg.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://efm.meibo888.top

Go:   // 手写 map[T]int
来源：http://xhy.vehdjk.com

Ruby: arr.tally
来源：http://xho.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rfw.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://wue.chenlongwang.top

Py:   x in arr
来源：http://olh.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://qto.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://ovh.hcnkem.com

TS:   arr.includes(x)
来源：http://gzj.zhongyouzk.top

Java: list.contains(x)
来源：http://lmf.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://msf.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://hsi.hnxiangtu.top

C#:   list.Contains(x)
来源：http://gft.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://vpu.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fzz.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nup.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://okj.gotoacloud.top

TS:   [...arr];
来源：http://vhs.zycfv.cn

Java: new ArrayList<>(list);
来源：http://yce.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ngq.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://kxh.daxiang520.top

C#:   new List<int>(list);
来源：http://lxx.0kj1m.cn

[D23] reduce 累积计算
来源：http://zqc.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bvi.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rfz.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zsd.gaohongyu789.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvb.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wuq.nanxinkj.top

Go:   // 手写循环
来源：http://nog.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wju.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qqt.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://ddc.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rwr.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfk.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ups.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qid.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ppc.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://czg.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pim.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ycr.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://quo.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ymi.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sqo.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wrt.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mqy.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://grs.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://feo.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gah.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yet.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://jon.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://mky.birdmap.top

PHP:  implode(", ", $arr);
来源：http://oar.fzhhl.top

JS:   arr.join(", ")
来源：http://cjm.snrcjt.cn

TS:   arr.join(", ")
来源：http://dte.zhengqikj.top

Java: String.join(", ", list)
来源：http://iau.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://llp.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://nix.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://goy.andypj.xyz

================================================================================
来源：http://irw.chenzaomai.com

E. 字符串处理
来源：http://tht.shanyushiyangtech.top

================================================================================
来源：http://afi.havefunace.top

[E01] 拼接字符串
来源：http://ath.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kdk.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://brv.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwn.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qkc.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://afi.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tka.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oeg.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ygz.9152youxi.cn

[E02] 重复字符串
来源：http://rvz.quarkkingdee.top

Py:   "ab" * 3
来源：http://vio.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://alj.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://dhp.yvedp.cn

TS:   "ab".repeat(3)
来源：http://uil.fzhhl.top

Java: "ab".repeat(3)
来源：http://jhn.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://auf.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://ndr.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://saq.sxryk.cn

[E03] 截取子串
来源：http://gje.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ozi.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gtk.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bcb.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://zxo.chenzaomai.com

Java: s.substring(1, 4)
来源：http://dyt.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cgu.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://tgn.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://dld.hcnkem.com

[E04] 查找子串位置
来源：http://dgn.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://hsb.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://sre.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fla.hywenlv.cn

TS:   s.indexOf("x")
来源：http://lqx.birdmap.top

Java: s.indexOf("x")
来源：http://qoh.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://fnb.hongshengwenyu.top

Ruby: s.index("x")
来源：http://btv.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://ooc.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aoj.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kfm.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wkm.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqb.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jyb.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cyo.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jbq.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jem.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bev.vqdsnc.cn

[E06] 替换子串
来源：http://ksu.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jso.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://buv.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://spc.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://yrd.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pfs.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lun.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bch.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://biu.ehwqpu.com

[E07] 按分隔符拆分
来源：http://kpz.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wnb.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fzo.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jey.xylfe.cn

TS:   s.split(",")
来源：http://vlj.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://xup.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nra.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://vrw.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bpl.fengsongda.top

[E08] 数组按分隔符合并
来源：http://ska.tarul.cn

Py:   ",".join(items)
来源：http://jao.ppjwa.cn

PHP:  implode(",", $items);
来源：http://hov.iojbl.cn

JS:   items.join(",")
来源：http://onp.daxiang520.top

TS:   items.join(",")
来源：http://phj.wangdashe.top

Java: String.join(",", items)
来源：http://voy.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://klr.tian-w.cn

Ruby: items.join(",")
来源：http://ovb.yfazqb.com

C#:   string.Join(",", items)
来源：http://lkv.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://jwl.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jqp.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gaq.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://dsy.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://bao.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://ken.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://twa.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://obe.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rvy.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://mfm.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hdw.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rqy.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://uvt.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://vel.daxiang520.top

Java: String.format("%03d", 7)
来源：http://uaz.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://qfo.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ymm.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iat.cucudq.cn

[E11] 反转字符串
来源：http://cyk.haohaochexian.top

Py:   s[::-1]
来源：http://ofq.svipenyu.cn

PHP:  strrev($s);
来源：http://wjg.nwbrower.top


<!-- 参考信息 -->