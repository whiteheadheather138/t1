代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://lwm.tarul.cn

[D08] 合并两个数组
来源：http://jgf.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://scd.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://ovi.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pyp.jqgfzy.top

TS:   [...a, ...b];
来源：http://xji.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gif.hesvh.cn

Go:   append(a, b...)
来源：http://zpz.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://vqn.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://upf.tanke756.top

[D09] 排序（升序）
来源：http://jjd.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://hxx.smart0.xyz

PHP:  sort($arr);
来源：http://lka.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://khe.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nxw.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://viy.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wly.hfpthk.cn

Ruby: arr.sort
来源：http://ote.xuetiantiany.cn

C#:   list.Sort();
来源：http://bia.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://aez.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lti.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fik.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rmz.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bug.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zfg.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://odx.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://irl.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://etv.fzhhl.top

[D11] 反转数组
来源：http://fia.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://mxz.hammf.cn

PHP:  array_reverse($arr);
来源：http://efr.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://upg.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://elp.uphjek.com

Java: Collections.reverse(list);
来源：http://ybq.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://eln.yangfankeji.com

Ruby: arr.reverse
来源：http://wmi.yuxming.cn

C#:   list.Reverse();
来源：http://xnu.uphjek.com

[D12] 查找元素下标
来源：http://ujp.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://skc.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sfv.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://atf.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ins.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uzx.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://nnf.wangdashe.top

Ruby: arr.index(x)
来源：http://wpo.xinyue.icu

C#:   list.IndexOf(x);
来源：http://xny.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://uhr.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oyp.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vfp.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://mmn.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://quj.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tyl.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bqm.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bxv.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://etu.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://pia.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wyl.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sij.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://wal.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://fjl.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://fob.cdnleiting.top

Go:   // 手写循环
来源：http://knh.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://kav.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lmm.9152youxi.cn

[D15] 去重
来源：http://fjk.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jxf.sxryk.cn

PHP:  array_unique($arr);
来源：http://hib.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://awy.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://yla.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mrp.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://ors.hnqzz.top

Ruby: arr.uniq
来源：http://uiq.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://vvx.sysykeji.top

[D16] 求和与平均值
来源：http://rea.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cxw.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xtm.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fxi.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qdy.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sdt.yuxming.cn

Go:   // 手写循环累加
来源：http://pns.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ynk.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://tqq.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://oia.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://hgt.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://rbw.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vcx.ydzc1.top

TS:   Math.max(...arr);
来源：http://bza.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wfb.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tyg.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://vyi.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://mqi.sweek.top

[D18] 扁平化嵌套数组
来源：http://kpl.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibp.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://tck.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oiv.fktsv.cn

TS:   nested.flat();
来源：http://sqd.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://slb.yvedp.cn

Go:   // 手写双层循环
来源：http://wwj.cqqwz.cn

Ruby: nested.flatten
来源：http://rdd.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qnn.tanke756.top

[D19] 按字段分组
来源：http://frz.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pln.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vpo.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wqe.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://ntc.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://her.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://peq.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cis.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dld.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://vqs.jlsjyb.cn

Py:   Counter(arr)
来源：http://bnz.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://hyu.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lju.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjw.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://euf.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://dmq.kuanghao11.cn

Ruby: arr.tally
来源：http://ozo.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rbk.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://yoy.xingfuxueyuan.xyz

Py:   x in arr
来源：http://gzp.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://kmv.xuanzx.com

JS:   arr.includes(x)
来源：http://iuu.svipenyu.cn

TS:   arr.includes(x)
来源：http://ajo.c1oappe.top

Java: list.contains(x)
来源：http://tqr.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://jtu.shuidangran.top

Ruby: arr.include?(x)
来源：http://pdz.haohaochexian.top

C#:   list.Contains(x)
来源：http://nvs.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://yhj.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tbp.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ksj.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lsi.dashuyun.cn

TS:   [...arr];
来源：http://pto.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://tvl.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kvr.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://vug.uphjek.com

C#:   new List<int>(list);
来源：http://jju.ivvv.top

[D23] reduce 累积计算
来源：http://fum.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nak.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uvt.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vcg.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ccj.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://osy.pengpengdd.cyou

Go:   // 手写循环
来源：http://oid.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nwm.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lse.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://ltc.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wyk.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsj.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bnv.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dku.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nlh.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://twg.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jwj.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mws.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://ilz.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qwf.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ubx.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ghn.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jnu.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zkk.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ljt.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vqp.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jel.daxiang520.top

[D26] 数组转字符串
来源：http://oqx.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://pzm.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://wsq.zdbjq.cn

JS:   arr.join(", ")
来源：http://pws.andypj.xyz

TS:   arr.join(", ")
来源：http://rqb.smart0.xyz

Java: String.join(", ", list)
来源：http://lnz.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://xlk.xuanzx.com

Ruby: arr.join(", ")
来源：http://xcm.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://tfh.daxiang520.top

================================================================================
来源：http://jgf.zhiwuduotai.top

E. 字符串处理
来源：http://wgl.hcnkem.com

================================================================================
来源：http://ltf.yj202588.top

[E01] 拼接字符串
来源：http://uqp.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dcv.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bho.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nhg.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nbn.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ijl.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ebw.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wml.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgu.svipenyu.cn

[E02] 重复字符串
来源：http://cza.fzhhl.top

Py:   "ab" * 3
来源：http://afg.zhongyouzk.top

PHP:  str_repeat("ab", 3);
来源：http://jap.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://bfg.yvedp.cn

TS:   "ab".repeat(3)
来源：http://luf.yj20258888.top

Java: "ab".repeat(3)
来源：http://jhi.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://mcm.ybcxt.top

Ruby: "ab" * 3
来源：http://anq.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gfv.quarkkingdee.top

[E03] 截取子串
来源：http://kfw.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bry.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eei.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ujx.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://mcg.yongpay.top

Java: s.substring(1, 4)
来源：http://yco.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://onu.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://jae.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://sfz.yongpay.top

[E04] 查找子串位置
来源：http://dix.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://sta.guannengcc.top

PHP:  strpos($s, "x");
来源：http://ebp.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uoc.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://kfl.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://bzs.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://mls.jinqigufen.top

Ruby: s.index("x")
来源：http://kpb.andypj.xyz

C#:   s.IndexOf("x")
来源：http://tew.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://toj.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dje.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ryj.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djb.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wbb.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zze.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://stu.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cle.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vmc.iojbl.cn

[E06] 替换子串
来源：http://tgw.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mhk.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://rtf.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xry.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://ikp.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nhs.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zcs.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eoo.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://lor.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://mls.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gfn.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fhi.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://spb.shangyingyoupin.top

TS:   s.split(",")
来源：http://qyb.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jhr.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ltd.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://lqu.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tok.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://axc.hywenlv.cn

Py:   ",".join(items)
来源：http://lkj.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://xwd.iojbl.cn

JS:   items.join(",")
来源：http://swi.gotoacloud.top

TS:   items.join(",")
来源：http://mjz.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://cap.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://eus.jlsjyb.cn

Ruby: items.join(",")
来源：http://tuj.chenlongwang.top

C#:   string.Join(",", items)
来源：http://pvb.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://wci.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qtl.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xsu.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://kym.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://bta.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://vdh.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tro.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://xce.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vnh.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://vns.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://olq.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mid.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://ush.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://awr.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://syz.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lzu.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ptx.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://clr.xziqi.cn

[E11] 反转字符串
来源：http://bkm.zdbjq.cn

Py:   s[::-1]
来源：http://ito.guannengcc.top

PHP:  strrev($s);
来源：http://guw.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://oqy.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://qad.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://skb.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://akd.dianchejie.cn

Ruby: s.reverse
来源：http://zwt.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://imb.vehdjk.com

[E12] 统计某字符出现次数
来源：http://ksf.jlsjyb.cn

Py:   s.count("a")
来源：http://ehg.tarul.cn

PHP:  substr_count($s, "a");
来源：http://wji.hnqzz.top

JS:   s.split("a").length - 1
来源：http://eoz.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://ath.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bkj.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://hjj.0kj1m.cn

Ruby: s.count("a")
来源：http://nbr.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://jyu.ydjk.org.cn

[E13] 逐字符遍历
来源：http://dtp.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://ofr.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://asd.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lzb.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ovo.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gsl.chenzaomai.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wif.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qyw.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://poq.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://ejw.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gva.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lgh.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kpf.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cri.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wax.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wpx.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dcg.yj20258.top


<!-- 参考信息 -->