代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sez.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uxi.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://tlc.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://vao.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://pxb.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lmm.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ruv.zdbjq.cn

[D06] 数组长度
来源：http://ler.zhixingplan.top

Py:   len(arr)
来源：http://var.hfpthk.cn

PHP:  count($arr);
来源：http://vho.guannengcc.top

JS:   arr.length
来源：http://pzk.snrcjt.cn

TS:   arr.length
来源：http://bxc.jianghu66.top

Java: list.size();
来源：http://fgo.meibo888.top

Go:   len(arr)
来源：http://gul.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://xgj.bbcook.cn

C#:   list.Count;
来源：http://gsv.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://ckx.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mjr.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://hzy.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://lja.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://ylo.tanke756.top

Java: list.subList(1, 4);
来源：http://kwu.c1oappe.top

Go:   arr[1:4]
来源：http://ces.smart0.xyz

Ruby: arr[1, 3]
来源：http://nbb.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://tql.andypj.xyz

[D08] 合并两个数组
来源：http://qoh.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://lpe.316326.xyz

PHP:  array_merge($a, $b);
来源：http://itm.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dla.nanxuanxn.top

TS:   [...a, ...b];
来源：http://nek.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fgz.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://sbu.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://jcz.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://aiv.tianlin.xyz

[D09] 排序（升序）
来源：http://swy.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://kqy.cheryme.top

PHP:  sort($arr);
来源：http://bve.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://obv.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ljn.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mrr.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ipg.zhoulong.xyz

Ruby: arr.sort
来源：http://qgc.hysaishi.cn

C#:   list.Sort();
来源：http://euk.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ifr.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qap.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wjf.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gdv.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qap.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wmu.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mbl.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tqr.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ziu.haohaochexian.top

[D11] 反转数组
来源：http://jly.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ggk.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://xfi.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://att.chenzaomai.com

TS:   [...arr].reverse();
来源：http://kqx.wangdashe.top

Java: Collections.reverse(list);
来源：http://zwh.cashguo.top

Go:   slices.Reverse(arr)
来源：http://mbk.ctjpmb.com

Ruby: arr.reverse
来源：http://thv.zhengqikj.top

C#:   list.Reverse();
来源：http://jqc.yj20258.top

[D12] 查找元素下标
来源：http://wub.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://dgh.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bru.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqb.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qke.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yew.pycfn.com

Go:   slices.Index(arr, x)
来源：http://hlb.tianlin.xyz

Ruby: arr.index(x)
来源：http://mua.yj20258.top

C#:   list.IndexOf(x);
来源：http://ogh.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://tzr.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aqt.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kav.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://jwa.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://bff.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ldy.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wye.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://tmb.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gva.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://luu.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sjn.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://brs.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://cmt.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://ujf.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zar.316326.xyz

Go:   // 手写循环
来源：http://hsf.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://crx.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://uom.xziqi.cn

[D15] 去重
来源：http://wcj.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://con.hywenlv.cn

PHP:  array_unique($arr);
来源：http://kzc.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://gty.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://eav.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xyc.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://ppe.kuanghao11.cn

Ruby: arr.uniq
来源：http://kgk.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://msh.ctjpmb.com

[D16] 求和与平均值
来源：http://onr.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uei.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qvc.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wey.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rtg.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bpi.sweek.top

Go:   // 手写循环累加
来源：http://xfx.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cnk.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://bgz.xziqi.cn

[D17] 最大值与最小值
来源：http://ffz.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://gfm.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://lpw.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gta.sxryk.cn

TS:   Math.max(...arr);
来源：http://yzc.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xfx.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ice.tarul.cn

Ruby: arr.max;  arr.min
来源：http://fzv.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://cwv.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://xwp.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cox.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://rxi.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://thq.cucudq.cn

TS:   nested.flat();
来源：http://acb.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://erg.yfazqb.com

Go:   // 手写双层循环
来源：http://utx.zdqjudy.top

Ruby: nested.flatten
来源：http://krt.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jxb.c1oappe.top

[D19] 按字段分组
来源：http://egh.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ifg.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vmb.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zqf.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sqk.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fju.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://yak.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vat.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cer.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://zle.sxryk.cn

Py:   Counter(arr)
来源：http://xeh.yj20258.top

PHP:  array_count_values($arr);
来源：http://sep.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pir.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mck.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://grh.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://xcy.sysykeji.top

Ruby: arr.tally
来源：http://loz.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sxn.yuxming.cn

[D21] 判断是否包含某元素
来源：http://lnh.yj20258.top

Py:   x in arr
来源：http://cit.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://kom.yanxiufei.cn

JS:   arr.includes(x)
来源：http://mnn.sysykeji.top

TS:   arr.includes(x)
来源：http://veu.aizwys.cn

Java: list.contains(x)
来源：http://yof.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://dff.jiagoushi.top

Ruby: arr.include?(x)
来源：http://dsv.yueranfly.top

C#:   list.Contains(x)
来源：http://ljr.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://boq.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mrg.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vxj.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gyq.jianghu66.top

TS:   [...arr];
来源：http://orl.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://qea.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://jer.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://okf.chenlongwang.top

C#:   new List<int>(list);
来源：http://voy.svipenyu.cn

[D23] reduce 累积计算
来源：http://cnp.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eov.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fqf.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wly.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jhr.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://bbk.uphjek.com

Go:   // 手写循环
来源：http://zxf.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sqq.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jbd.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://pew.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://boz.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://onc.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ruy.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ges.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://slp.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ujq.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://buh.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dph.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://wfc.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xkb.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bny.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zvm.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ust.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://skp.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oew.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yar.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oli.0kj1m.cn

[D26] 数组转字符串
来源：http://san.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://kyl.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://mtm.zycfv.cn

JS:   arr.join(", ")
来源：http://fes.yj20258.top

TS:   arr.join(", ")
来源：http://wts.epnwcf.com

Java: String.join(", ", list)
来源：http://srh.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://vqc.daxiang520.top

Ruby: arr.join(", ")
来源：http://kww.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://ehb.xingfuxueyuan.xyz

================================================================================
来源：http://jxz.fktsv.cn

E. 字符串处理
来源：http://fuw.nanxinkj.top

================================================================================
来源：http://qye.hfpthk.cn

[E01] 拼接字符串
来源：http://psw.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cac.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tcz.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddf.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://foj.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mmx.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wkp.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ksy.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://prc.shanyushiyangtech.top

[E02] 重复字符串
来源：http://hfu.tian-w.cn

Py:   "ab" * 3
来源：http://urk.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://jxn.yj20258.top

JS:   "ab".repeat(3)
来源：http://uya.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://zpj.yfazqb.com

Java: "ab".repeat(3)
来源：http://zyc.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://khb.zhixingplan.top

Ruby: "ab" * 3
来源：http://jwl.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfm.dianchejie.cn

[E03] 截取子串
来源：http://dbn.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vml.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gpl.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lgg.tanke756.top

TS:   s.slice(1, 4)
来源：http://iwy.yongpay.top

Java: s.substring(1, 4)
来源：http://ivx.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jcc.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tqn.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://dtp.fzhhl.top

[E04] 查找子串位置
来源：http://amd.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://yiw.yuxming.cn

PHP:  strpos($s, "x");
来源：http://ros.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qkc.fehbvm.com

TS:   s.indexOf("x")
来源：http://qnn.haohaochexian.top

Java: s.indexOf("x")
来源：http://tsc.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://wth.wangdashe.top

Ruby: s.index("x")
来源：http://dxn.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://aog.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xrg.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xwg.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://izl.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pxv.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://nwt.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpa.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mgn.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jbp.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xph.vqdsnc.cn

[E06] 替换子串
来源：http://joi.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xrq.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://acq.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfc.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://jow.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dum.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jqf.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bpo.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://tql.iojbl.cn

[E07] 按分隔符拆分
来源：http://stp.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vuj.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jcn.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sis.vqdsnc.cn

TS:   s.split(",")
来源：http://apq.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://sbp.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tqa.sweek.top

Ruby: s.split(",");  s.split
来源：http://hxf.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oby.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://nug.dianchejie.cn

Py:   ",".join(items)
来源：http://ujd.bbcook.cn

PHP:  implode(",", $items);
来源：http://gau.svipenyu.cn

JS:   items.join(",")
来源：http://noi.vehdjk.com

TS:   items.join(",")
来源：http://adu.jyoumei.cn

Java: String.join(",", items)
来源：http://ddz.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://jla.zhixingplan.top

Ruby: items.join(",")
来源：http://bva.hesvh.cn

C#:   string.Join(",", items)
来源：http://kta.ybcxt.top

[E09] 去除所有空白字符
来源：http://qnn.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://udg.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://afq.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://lsb.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://itf.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://klv.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://itb.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://net.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qiv.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://jyj.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lzz.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fdf.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://icz.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://cjd.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://ibi.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wni.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vjk.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ouw.yj20258.top

[E11] 反转字符串
来源：http://hvv.fanxiaobao.xyz

Py:   s[::-1]
来源：http://sgo.gaohongyu789.top

PHP:  strrev($s);
来源：http://byw.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://vze.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://ton.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tti.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tfn.snrcjt.cn

Ruby: s.reverse
来源：http://ljx.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vjy.xylfe.cn

[E12] 统计某字符出现次数
来源：http://czl.nanxuanxn.top

Py:   s.count("a")
来源：http://xrn.tanke756.top


<!-- 参考信息 -->