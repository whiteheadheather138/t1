代发 wailian999

[D07] 切片 / 取子数组
来源：http://hxx.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rxh.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://ygr.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://uzi.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://gzx.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://bpm.0kj1m.cn

Go:   arr[1:4]
来源：http://fvt.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://gwy.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://cwf.ydjk.org.cn

[D08] 合并两个数组
来源：http://rjm.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://kur.sweek.top

PHP:  array_merge($a, $b);
来源：http://vil.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ihv.xinyue.icu

TS:   [...a, ...b];
来源：http://hbq.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kqt.smart0.xyz

Go:   append(a, b...)
来源：http://vno.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://kxv.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://hqm.tarul.cn

[D09] 排序（升序）
来源：http://rkl.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://aei.xuanzx.com

PHP:  sort($arr);
来源：http://dbd.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rud.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lzg.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bro.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zak.hysaishi.cn

Ruby: arr.sort
来源：http://wgu.jlsjyb.cn

C#:   list.Sort();
来源：http://xjg.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://shq.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lbm.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gtn.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bts.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ujv.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lou.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://npl.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dbx.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pwd.cdnleiting.top

[D11] 反转数组
来源：http://vhr.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ybo.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://axj.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qkt.hywenlv.cn

TS:   [...arr].reverse();
来源：http://qgd.zycfv.cn

Java: Collections.reverse(list);
来源：http://cpi.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://hyo.kuanghao11.cn

Ruby: arr.reverse
来源：http://irs.jianghu66.top

C#:   list.Reverse();
来源：http://qwp.shuidangran.top

[D12] 查找元素下标
来源：http://ddb.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://cqo.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hja.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://btj.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxp.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yvw.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://kjd.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://zwh.vehdjk.com

C#:   list.IndexOf(x);
来源：http://stk.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://men.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lvn.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jyc.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://jfe.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://kkl.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qyt.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vzu.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://hyf.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ktq.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://vjj.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://srs.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jkr.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://vcq.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://gua.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tgj.hywenlv.cn

Go:   // 手写循环
来源：http://iri.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://iqx.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://omg.uphjek.com

[D15] 去重
来源：http://myx.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hiv.0kj1m.cn

PHP:  array_unique($arr);
来源：http://jdm.xylfe.cn

JS:   [...new Set(arr)]
来源：http://vhx.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://upq.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpa.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://rui.guowangkeji.top

Ruby: arr.uniq
来源：http://oek.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://epl.yangfankeji.com

[D16] 求和与平均值
来源：http://abe.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://utz.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iiv.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qhq.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xoo.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qhw.shzxlz.cn

Go:   // 手写循环累加
来源：http://mnu.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wso.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://xkx.epnwcf.com

[D17] 最大值与最小值
来源：http://gjz.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://eoj.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://lnm.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mwx.bbcook.cn

TS:   Math.max(...arr);
来源：http://qfx.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fks.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vda.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://hyr.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://oqx.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://dqu.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ijn.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://com.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jgq.zdqjudy.top

TS:   nested.flat();
来源：http://esv.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jqk.hysaishi.cn

Go:   // 手写双层循环
来源：http://rut.316326.xyz

Ruby: nested.flatten
来源：http://dmo.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hpw.sxryk.cn

[D19] 按字段分组
来源：http://rhz.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://skm.cheryme.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dgg.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wsh.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wrk.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ucp.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://joc.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ueo.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zol.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://gog.guowangkeji.top

Py:   Counter(arr)
来源：http://hug.yonumen.top

PHP:  array_count_values($arr);
来源：http://qum.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ffv.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gzl.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://inm.yuxming.cn

Go:   // 手写 map[T]int
来源：http://qgp.quarkkingdee.top

Ruby: arr.tally
来源：http://ruq.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://den.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://mfp.daria6918.cn

Py:   x in arr
来源：http://uls.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://rea.smart0.xyz

JS:   arr.includes(x)
来源：http://uqo.yvedp.cn

TS:   arr.includes(x)
来源：http://zti.aibaodan.cn

Java: list.contains(x)
来源：http://ini.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://bgz.epnwcf.com

Ruby: arr.include?(x)
来源：http://nwq.0kj1m.cn

C#:   list.Contains(x)
来源：http://lrv.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://wrk.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://prn.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rog.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hiv.hcnkem.com

TS:   [...arr];
来源：http://ftj.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://acs.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dct.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://aal.sufxvd.cn

C#:   new List<int>(list);
来源：http://mba.jinqigufen.top

[D23] reduce 累积计算
来源：http://ugq.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lbm.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dbr.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vae.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://afq.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vvu.gogol.net.cn

Go:   // 手写循环
来源：http://pwf.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vnx.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uel.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://kfn.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sih.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://phw.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ret.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dbn.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rjy.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wmg.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wfe.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mqk.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://bck.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sdd.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bju.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bjo.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iqy.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wth.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ygz.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dbt.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nfr.tian-w.cn

[D26] 数组转字符串
来源：http://lvs.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://oxz.meibo888.top

PHP:  implode(", ", $arr);
来源：http://qyj.snrcjt.cn

JS:   arr.join(", ")
来源：http://mwv.dianchejie.cn

TS:   arr.join(", ")
来源：http://tre.ydjk.org.cn

Java: String.join(", ", list)
来源：http://enw.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://kji.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://fvg.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://gbj.yonumen.top

================================================================================
来源：http://rcc.jinqigufen.top

E. 字符串处理
来源：http://puj.yonumen.top

================================================================================
来源：http://mqf.aizwys.cn

[E01] 拼接字符串
来源：http://knz.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nky.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cxj.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nis.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hno.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jvy.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nkn.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gej.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bep.sufxvd.cn

[E02] 重复字符串
来源：http://dki.smart0.xyz

Py:   "ab" * 3
来源：http://kez.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://gzu.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://lmp.meibo888.top

TS:   "ab".repeat(3)
来源：http://zzo.hfpthk.cn

Java: "ab".repeat(3)
来源：http://val.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://evm.xinyue.icu

Ruby: "ab" * 3
来源：http://dgf.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://swn.meibo888.top

[E03] 截取子串
来源：http://rfl.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://skn.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://noq.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vqe.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://ukx.ivvv.top

Java: s.substring(1, 4)
来源：http://obd.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://byr.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://oov.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://hhq.gaohongyu789.top

[E04] 查找子串位置
来源：http://igb.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://xzo.cucudq.cn

PHP:  strpos($s, "x");
来源：http://xoz.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pxx.nanxinkj.top

TS:   s.indexOf("x")
来源：http://awb.pycfn.com

Java: s.indexOf("x")
来源：http://vrl.yj20258.top

Go:   strings.Index(s, "x")
来源：http://ter.yj20258888.top

Ruby: s.index("x")
来源：http://ykz.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://yki.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kft.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ohb.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyw.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://phe.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dgg.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rlu.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kic.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zoi.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lgt.shanyushiyangkeji.top

[E06] 替换子串
来源：http://isk.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rcy.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://zrg.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rov.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://bzq.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jku.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kdr.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://luu.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://vsw.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://afy.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iea.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ijs.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bwl.mhx1999.top

TS:   s.split(",")
来源：http://icw.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dew.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xhe.hammf.cn

Ruby: s.split(",");  s.split
来源：http://hux.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bsk.meibo888.top

[E08] 数组按分隔符合并
来源：http://akm.tianlin.xyz

Py:   ",".join(items)
来源：http://foe.tian-w.cn

PHP:  implode(",", $items);
来源：http://rwe.shanyushiyangtech.top

JS:   items.join(",")
来源：http://xao.jyoumei.cn

TS:   items.join(",")
来源：http://fky.chenzaomai.com

Java: String.join(",", items)
来源：http://ylm.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://tso.yvedp.cn

Ruby: items.join(",")
来源：http://hoo.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://hus.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://dip.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qbm.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xek.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://gwt.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://pwt.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://nan.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wwy.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://frl.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hcm.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://tlc.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dpn.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wbp.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://ull.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://qou.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://ael.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uqe.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://khp.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dia.ctjpmb.com

[E11] 反转字符串
来源：http://iiw.0kj1m.cn

Py:   s[::-1]
来源：http://mwy.jlsjyb.cn

PHP:  strrev($s);
来源：http://ewu.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://wva.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://nzm.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dxt.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lrp.guannengcc.top

Ruby: s.reverse
来源：http://wat.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pho.hesvh.cn

[E12] 统计某字符出现次数
来源：http://zys.hcnkem.com

Py:   s.count("a")
来源：http://cmd.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://juh.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://oyb.xuanzx.com

TS:   s.split("a").length - 1
来源：http://mdo.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fbr.uphjek.com

Go:   strings.Count(s, "a")
来源：http://axu.cheryme.top

Ruby: s.count("a")
来源：http://iee.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://sxo.bjfxy.top

[E13] 逐字符遍历
来源：http://rmg.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://pyw.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://izs.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gbz.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://gmj.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hzp.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://umj.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sqp.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zno.shanyushiyangtech.top


<!-- 参考信息 -->