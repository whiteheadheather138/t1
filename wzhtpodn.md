代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lmp.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://osh.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qwo.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aup.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qcj.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fyw.jinqigfzy.top

[D05] 访问与修改元素
来源：http://ylx.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ttk.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rdq.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nai.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://kzq.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://nme.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://kck.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xrf.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://giz.hfpthk.cn

[D06] 数组长度
来源：http://mes.ivvv.top

Py:   len(arr)
来源：http://mca.gaohongyu789.top

PHP:  count($arr);
来源：http://tat.nwbrower.top

JS:   arr.length
来源：http://tzd.c1oappe.top

TS:   arr.length
来源：http://haf.cheryme.top

Java: list.size();
来源：http://eww.yuanzhike.top

Go:   len(arr)
来源：http://tih.andypj.xyz

Ruby: arr.length; arr.size
来源：http://tge.316326.xyz

C#:   list.Count;
来源：http://abe.iojbl.cn

[D07] 切片 / 取子数组
来源：http://mkb.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zvn.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xzi.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://smi.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://bmc.zdbjq.cn

Java: list.subList(1, 4);
来源：http://ccn.mhx1999.top

Go:   arr[1:4]
来源：http://gxl.gzhubu.top

Ruby: arr[1, 3]
来源：http://pjc.sweek.top

C#:   list.GetRange(1, 3);
来源：http://epf.jlsjyb.cn

[D08] 合并两个数组
来源：http://cmb.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://vbu.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://kmw.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zjc.zhijiandao.cn

TS:   [...a, ...b];
来源：http://agu.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eqf.9152youxi.cn

Go:   append(a, b...)
来源：http://til.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://osb.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://vuk.ydzc1.top

[D09] 排序（升序）
来源：http://jzt.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://whp.ctjpmb.com

PHP:  sort($arr);
来源：http://mfk.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xrt.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rmk.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kzx.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oge.xuanzx.com

Ruby: arr.sort
来源：http://cyi.daxiang520.top

C#:   list.Sort();
来源：http://gbj.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://szm.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tcs.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mmg.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jjd.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qip.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mkw.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://skx.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zzw.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dss.xuetiantiany.cn

[D11] 反转数组
来源：http://esc.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://gai.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://bil.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gix.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://ifd.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://yiu.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://imn.fehbvm.com

Ruby: arr.reverse
来源：http://xak.smart0.xyz

C#:   list.Reverse();
来源：http://gej.yfazqb.com

[D12] 查找元素下标
来源：http://hpl.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://zgv.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nas.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hbk.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kzt.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ltx.316326.xyz

Go:   slices.Index(arr, x)
来源：http://zsc.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://tox.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://svz.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://meb.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rgh.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gfp.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://cka.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://hgo.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bkc.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wzs.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://ttq.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cms.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://eyn.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://auv.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zsv.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://kyp.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://oxn.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sdi.9152youxi.cn

Go:   // 手写循环
来源：http://kth.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://puv.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dgv.chenzaomai.com

[D15] 去重
来源：http://tac.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xas.bbcook.cn

PHP:  array_unique($arr);
来源：http://ymm.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://jxl.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://drr.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yba.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vwz.dianchejie.cn

Ruby: arr.uniq
来源：http://esx.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://rtl.yj20258888.top

[D16] 求和与平均值
来源：http://xtm.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ncr.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://btt.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gnv.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://svd.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kol.zhoulong.xyz

Go:   // 手写循环累加
来源：http://ssv.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://frs.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://llk.sweek.top

[D17] 最大值与最小值
来源：http://mht.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://dix.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://nuq.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://npn.chenlongwang.top

TS:   Math.max(...arr);
来源：http://xcj.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://huc.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cgu.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://yqh.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://qdc.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://jeu.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vdq.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://pfa.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mod.hnqzz.top

TS:   nested.flat();
来源：http://mwb.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lku.hywenlv.cn

Go:   // 手写双层循环
来源：http://jfz.xuanzx.com

Ruby: nested.flatten
来源：http://rpc.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tlw.birdmap.top

[D19] 按字段分组
来源：http://zha.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cix.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://owz.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lly.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uwa.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ple.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://lee.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mhc.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dzn.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://aam.gaohongyu789.top

Py:   Counter(arr)
来源：http://wnv.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://mxu.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jqi.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bfd.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://otc.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://bmt.zhixingplan.top

Ruby: arr.tally
来源：http://tzq.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yqd.sweek.top

[D21] 判断是否包含某元素
来源：http://hpu.sysykeji.top

Py:   x in arr
来源：http://izw.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://bom.guowangkeji.top

JS:   arr.includes(x)
来源：http://dgl.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://iaj.yj20258888.top

Java: list.contains(x)
来源：http://hgn.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://xzt.ybcxt.top

Ruby: arr.include?(x)
来源：http://pnp.wangdashe.top

C#:   list.Contains(x)
来源：http://lwg.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://kxf.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://low.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dnm.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rdr.chenlongwang.top

TS:   [...arr];
来源：http://png.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://sjj.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://oec.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://ruw.yonumen.top

C#:   new List<int>(list);
来源：http://vrr.yj20258888.top

[D23] reduce 累积计算
来源：http://rnw.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gpl.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ykx.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfh.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fgh.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dyb.tianlin.xyz

Go:   // 手写循环
来源：http://stp.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nph.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dtm.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://sjf.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://syr.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dzx.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cvi.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://alb.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pfy.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pqh.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xoz.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hfk.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://ypw.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ynn.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://efv.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fso.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://usu.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kiy.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mfa.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://guz.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ugu.jlsjyb.cn

[D26] 数组转字符串
来源：http://ajo.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://oyd.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://cvr.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://yja.xuanzx.com

TS:   arr.join(", ")
来源：http://qgr.sweek.top

Java: String.join(", ", list)
来源：http://nvl.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://zkm.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://rue.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://khc.smart0.xyz

================================================================================
来源：http://vqr.havefunace.top

E. 字符串处理
来源：http://dhe.wangdashe.top

================================================================================
来源：http://hcp.gzhubu.top

[E01] 拼接字符串
来源：http://ymj.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jev.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ltf.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://els.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://acj.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://icj.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mbh.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uny.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xia.birdmap.top

[E02] 重复字符串
来源：http://swy.jiagoushi.top

Py:   "ab" * 3
来源：http://shn.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://qpl.mhx1999.top

JS:   "ab".repeat(3)
来源：http://fgl.yuxming.cn

TS:   "ab".repeat(3)
来源：http://cuj.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://etf.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://ari.xinyue.icu

Ruby: "ab" * 3
来源：http://kqa.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fol.gaohongyu789.top

[E03] 截取子串
来源：http://mjs.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fen.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eqt.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aha.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://lmn.hammf.cn

Java: s.substring(1, 4)
来源：http://tzt.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eka.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://amy.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://mxd.ybcxt.top

[E04] 查找子串位置
来源：http://wvw.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://umr.ydzc1.top

PHP:  strpos($s, "x");
来源：http://gss.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gem.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://mql.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://rlw.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://qhy.zhijiandao.cn

Ruby: s.index("x")
来源：http://iag.bjfxy.top

C#:   s.IndexOf("x")
来源：http://ont.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://ygb.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://utb.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nqr.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xhp.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xkx.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cpf.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://otw.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ziq.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nwh.yongpay.top

[E06] 替换子串
来源：http://ivw.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wwi.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://aqw.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwu.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://ney.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ulq.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cem.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tht.pycfn.com

C#:   s.Replace("a", "b")
来源：http://jga.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://kev.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rso.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ivm.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kge.kuanghao11.cn

TS:   s.split(",")
来源：http://nov.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tyj.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wme.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://hnk.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rfd.tian-w.cn

[E08] 数组按分隔符合并
来源：http://hsy.sysykeji.top

Py:   ",".join(items)
来源：http://zgb.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://qjo.zhengqikj.top

JS:   items.join(",")
来源：http://qvv.mhx1999.top

TS:   items.join(",")
来源：http://cjd.zdbjq.cn

Java: String.join(",", items)
来源：http://kwd.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://xjn.zhoulong.xyz

Ruby: items.join(",")
来源：http://bci.yueranfly.top

C#:   string.Join(",", items)
来源：http://lus.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://rcg.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nmo.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iat.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://jhn.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://vuv.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://yex.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jbb.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fuq.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sax.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://qhf.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qhj.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zpo.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://bjr.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://ucg.sxryk.cn

Java: String.format("%03d", 7)
来源：http://ntj.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jha.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://scm.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ywc.shuidangran.top

[E11] 反转字符串
来源：http://edr.yanxiufei.cn

Py:   s[::-1]
来源：http://rok.guowangkeji.top

PHP:  strrev($s);
来源：http://zmd.hesvh.cn


<!-- 参考信息 -->