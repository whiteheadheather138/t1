代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jah.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://izi.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://oeq.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://qha.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://man.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nxx.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dwj.iojbl.cn

[D06] 数组长度
来源：http://qtu.jiagoushi.top

Py:   len(arr)
来源：http://lmp.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://ing.guannengcc.top

JS:   arr.length
来源：http://avj.shanyushiyangtech.top

TS:   arr.length
来源：http://uok.yanxiufei.cn

Java: list.size();
来源：http://llh.yanxiufei.cn

Go:   len(arr)
来源：http://gwb.uphjek.com

Ruby: arr.length; arr.size
来源：http://lqz.smart0.xyz

C#:   list.Count;
来源：http://tmd.bjfxy.top

[D07] 切片 / 取子数组
来源：http://eus.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://akw.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://ikj.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://tsv.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://uxp.wangdashe.top

Java: list.subList(1, 4);
来源：http://rrs.yuxming.cn

Go:   arr[1:4]
来源：http://pxl.gzhubu.top

Ruby: arr[1, 3]
来源：http://saa.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://zxx.haohaochexian.top

[D08] 合并两个数组
来源：http://wey.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://xbg.yongpay.top

PHP:  array_merge($a, $b);
来源：http://jvy.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bgr.shuidangran.top

TS:   [...a, ...b];
来源：http://guh.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hmu.sjlbkw.cn

Go:   append(a, b...)
来源：http://xve.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://xrx.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://loc.yj20258888.top

[D09] 排序（升序）
来源：http://mze.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://flh.wangdashe.top

PHP:  sort($arr);
来源：http://hih.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wdb.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zxo.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://chr.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://peb.hcnkem.com

Ruby: arr.sort
来源：http://qys.yangfankeji.com

C#:   list.Sort();
来源：http://ulu.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lew.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jsa.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bbx.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cgi.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pvg.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yoe.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://stm.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qui.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rcw.yongpay.top

[D11] 反转数组
来源：http://xjf.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://vnd.vehdjk.com

PHP:  array_reverse($arr);
来源：http://eqh.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://edu.c1oappe.top

TS:   [...arr].reverse();
来源：http://kzg.nanxinkj.top

Java: Collections.reverse(list);
来源：http://xjl.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://eqx.svipenyu.cn

Ruby: arr.reverse
来源：http://paz.tanke756.top

C#:   list.Reverse();
来源：http://ifg.fktsv.cn

[D12] 查找元素下标
来源：http://ptm.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://cwi.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://toy.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugf.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tar.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://obx.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://glt.nanxuanxn.top

Ruby: arr.index(x)
来源：http://ebh.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://dto.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://nyd.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fxm.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ddn.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://wgi.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://nkk.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eas.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ahz.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zam.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pei.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://grs.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wdf.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cef.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://asw.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://cbl.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uct.yuxming.cn

Go:   // 手写循环
来源：http://yre.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ugv.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hjz.zycfv.cn

[D15] 去重
来源：http://rhv.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qbt.hammf.cn

PHP:  array_unique($arr);
来源：http://gaz.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://bhg.yj20258888.top

TS:   [...new Set(arr)]
来源：http://ymz.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uru.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wdb.hcnkem.com

Ruby: arr.uniq
来源：http://wtx.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://sol.cheryme.top

[D16] 求和与平均值
来源：http://gke.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bbr.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rnc.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://udv.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://asl.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sgl.shuidangran.top

Go:   // 手写循环累加
来源：http://dyl.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://edb.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://nzk.jinqigufen.top

[D17] 最大值与最小值
来源：http://tpy.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://nzd.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://ssz.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://frg.yvedp.cn

TS:   Math.max(...arr);
来源：http://cbg.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gjx.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jxl.tanke756.top

Ruby: arr.max;  arr.min
来源：http://oyi.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://dql.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://vte.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zlu.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://vbm.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://civ.yfazqb.com

TS:   nested.flat();
来源：http://xju.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mov.gotoacloud.top

Go:   // 手写双层循环
来源：http://hlh.shzxlz.cn

Ruby: nested.flatten
来源：http://xmb.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uyd.cashguo.top

[D19] 按字段分组
来源：http://ims.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ion.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://las.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ngu.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nwa.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iuf.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://rrf.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zfi.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lgg.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://obq.xylfe.cn

Py:   Counter(arr)
来源：http://frj.fengsongda.top

PHP:  array_count_values($arr);
来源：http://ifo.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltu.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vhm.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qjt.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://pdu.fengsongda.top

Ruby: arr.tally
来源：http://ywm.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oeo.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://rck.fengsongda.top

Py:   x in arr
来源：http://brx.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://fpl.yangfankeji.com

JS:   arr.includes(x)
来源：http://ezd.andypj.xyz

TS:   arr.includes(x)
来源：http://zdc.9152youxi.cn

Java: list.contains(x)
来源：http://znj.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://wlb.cqqwz.cn

Ruby: arr.include?(x)
来源：http://xoq.bbcook.cn

C#:   list.Contains(x)
来源：http://qqx.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://lxf.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ayd.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://phq.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zbv.fktsv.cn

TS:   [...arr];
来源：http://zsx.iojbl.cn

Java: new ArrayList<>(list);
来源：http://kem.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://cbi.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://ljf.fengsongda.top

C#:   new List<int>(list);
来源：http://mfs.zdqjudy.top

[D23] reduce 累积计算
来源：http://wdw.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zum.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hza.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kon.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xza.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fyh.aibaodan.cn

Go:   // 手写循环
来源：http://vqo.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fcm.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lyb.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://zya.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bvu.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vqk.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vmj.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tif.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rcm.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xgt.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jmt.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jvf.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://yuk.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rtj.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://afu.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ucl.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kho.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xpa.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nia.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rql.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dlx.pengpengdd.cyou

[D26] 数组转字符串
来源：http://mxz.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://tby.jiagoushi.top

PHP:  implode(", ", $arr);
来源：http://dqe.tanke756.top

JS:   arr.join(", ")
来源：http://sxq.xinyue.icu

TS:   arr.join(", ")
来源：http://bjm.quarkkingdee.top

Java: String.join(", ", list)
来源：http://deh.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://dex.ehwqpu.com

Ruby: arr.join(", ")
来源：http://tyf.sysykeji.top

C#:   string.Join(", ", list)
来源：http://pir.epnwcf.com

================================================================================
来源：http://fpk.svipenyu.cn

E. 字符串处理
来源：http://ycn.svipenyu.cn

================================================================================
来源：http://wtb.haohaochexian.top

[E01] 拼接字符串
来源：http://tgy.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jlx.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bsi.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zod.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jeb.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tje.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fyh.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jan.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uqi.yuanzhike.top

[E02] 重复字符串
来源：http://ijd.aibaodan.cn

Py:   "ab" * 3
来源：http://qde.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://emp.yj202588.top

JS:   "ab".repeat(3)
来源：http://ohr.316326.xyz

TS:   "ab".repeat(3)
来源：http://zjm.sysykeji.top

Java: "ab".repeat(3)
来源：http://usc.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://akt.ppjwa.cn

Ruby: "ab" * 3
来源：http://osb.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vje.yongpay.top

[E03] 截取子串
来源：http://rhk.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hbv.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sri.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ysa.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://qnd.dianchejie.cn

Java: s.substring(1, 4)
来源：http://dma.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lyl.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://arz.tarul.cn

C#:   s.Substring(1, 3)
来源：http://zko.chenzaomai.com

[E04] 查找子串位置
来源：http://moz.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://fju.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://var.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://igz.sxryk.cn

TS:   s.indexOf("x")
来源：http://swk.jyoumei.cn

Java: s.indexOf("x")
来源：http://bql.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://sqi.ydjk.org.cn

Ruby: s.index("x")
来源：http://rfm.mhx1999.top

C#:   s.IndexOf("x")
来源：http://rjp.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dva.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uwz.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ywu.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xiw.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://moz.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rjj.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kca.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgp.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://joe.fktsv.cn

[E06] 替换子串
来源：http://xzu.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bif.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://nbz.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbo.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://ava.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://phb.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kgz.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dcv.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://rzb.cucudq.cn

[E07] 按分隔符拆分
来源：http://ost.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjq.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zbg.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ygw.uphjek.com

TS:   s.split(",")
来源：http://cpc.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://tzb.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oiy.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://gjq.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mlm.shuidangran.top

[E08] 数组按分隔符合并
来源：http://jvt.sjlbkw.cn

Py:   ",".join(items)
来源：http://enm.guowangkeji.top

PHP:  implode(",", $items);
来源：http://qvr.yangfankeji.com

JS:   items.join(",")
来源：http://ael.ydzc1.top

TS:   items.join(",")
来源：http://joj.shangyingyoupin.top

Java: String.join(",", items)
来源：http://svq.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://gpu.cqqwz.cn

Ruby: items.join(",")
来源：http://pmf.guannengcc.top

C#:   string.Join(",", items)
来源：http://syn.0kj1m.cn

[E09] 去除所有空白字符
来源：http://nwk.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://edd.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mxv.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://cyp.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://dtd.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://gfk.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://awd.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://cbb.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ohi.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://lys.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kfp.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ygh.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://rvq.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://lmv.daxiang520.top

Java: String.format("%03d", 7)
来源：http://ntz.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ver.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cba.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://srm.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://sfz.nanxinkj.top

Py:   s[::-1]
来源：http://gxd.haohaochexian.top

PHP:  strrev($s);
来源：http://hmi.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://jqi.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://jra.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pfj.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://zab.ybcxt.top

Ruby: s.reverse
来源：http://atu.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://fzn.fzhhl.top

[E12] 统计某字符出现次数
来源：http://xvn.gotoacloud.top

Py:   s.count("a")
来源：http://qtk.tarul.cn


<!-- 参考信息 -->