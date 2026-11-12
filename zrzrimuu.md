代发 wailian999

Py:   len(arr)
来源：http://zud.gogol.net.cn

PHP:  count($arr);
来源：http://fru.zhengqikj.top

JS:   arr.length
来源：http://xeg.daria6918.cn

TS:   arr.length
来源：http://gaq.jiagoushi.top

Java: list.size();
来源：http://qyj.vqdsnc.cn

Go:   len(arr)
来源：http://aln.ivvv.top

Ruby: arr.length; arr.size
来源：http://gnj.yj20258888.top

C#:   list.Count;
来源：http://hom.jianghu66.top

[D07] 切片 / 取子数组
来源：http://ntd.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://edi.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ygq.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://zti.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://ksf.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://gkh.yuanzhike.top

Go:   arr[1:4]
来源：http://cva.xuanzx.com

Ruby: arr[1, 3]
来源：http://yfw.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://nun.aizwys.cn

[D08] 合并两个数组
来源：http://wxl.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://dmw.yongpay.top

PHP:  array_merge($a, $b);
来源：http://sqf.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lil.yj202588.top

TS:   [...a, ...b];
来源：http://vkw.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pqy.aizwys.cn

Go:   append(a, b...)
来源：http://loc.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://oof.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://xnt.birdmap.top

[D09] 排序（升序）
来源：http://ypd.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://cgj.wangdashe.top

PHP:  sort($arr);
来源：http://twt.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bcs.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xhi.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kbw.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cak.fktsv.cn

Ruby: arr.sort
来源：http://owm.zhengqikj.top

C#:   list.Sort();
来源：http://aef.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pei.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dlk.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hbi.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://txg.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wni.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rqj.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pef.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sae.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rpm.iojbl.cn

[D11] 反转数组
来源：http://cte.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ulz.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://mei.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tar.dianchejie.cn

TS:   [...arr].reverse();
来源：http://phg.xuanzx.com

Java: Collections.reverse(list);
来源：http://rar.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://fuw.birdmap.top

Ruby: arr.reverse
来源：http://vis.jyoumei.cn

C#:   list.Reverse();
来源：http://bts.ydjk.org.cn

[D12] 查找元素下标
来源：http://gjr.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://tnu.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hnw.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tyk.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bcy.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qam.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://wmk.ivvv.top

Ruby: arr.index(x)
来源：http://qca.316326.xyz

C#:   list.IndexOf(x);
来源：http://oqm.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://hwn.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://knv.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ydi.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://vov.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://pry.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dlk.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cvc.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iqn.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bon.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://kcy.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://brv.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://thz.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://wea.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://grn.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cmd.shangyingyoupin.top

Go:   // 手写循环
来源：http://ied.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://qgq.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bdg.zhiwuduotai.top

[D15] 去重
来源：http://syr.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ndn.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://lsn.vehdjk.com

JS:   [...new Set(arr)]
来源：http://jeg.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://gro.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://skr.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://mbv.andypj.xyz

Ruby: arr.uniq
来源：http://oag.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://nna.bjfxy.top

[D16] 求和与平均值
来源：http://kmj.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://abm.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ctd.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tmo.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yyk.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://huc.feifeiyinyue.top

Go:   // 手写循环累加
来源：http://hgw.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oqv.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://xjj.fktsv.cn

[D17] 最大值与最小值
来源：http://sws.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://pph.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://gvc.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fgn.havefunace.top

TS:   Math.max(...arr);
来源：http://fjn.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://muq.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vqy.uphjek.com

Ruby: arr.max;  arr.min
来源：http://iie.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://qar.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://jlk.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mvm.cheryme.top

PHP:  array_merge(...$nested);
来源：http://lba.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jru.hammf.cn

TS:   nested.flat();
来源：http://wht.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mfi.xuanzx.com

Go:   // 手写双层循环
来源：http://vbu.jlsjyb.cn

Ruby: nested.flatten
来源：http://fai.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://hqw.pycfn.com

[D19] 按字段分组
来源：http://aca.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pyi.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nrs.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ite.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hao.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dpl.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://jla.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bbm.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wso.sweek.top

[D20] 统计每个元素出现次数
来源：http://gbk.vqdsnc.cn

Py:   Counter(arr)
来源：http://bvz.sysykeji.top

PHP:  array_count_values($arr);
来源：http://hnj.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fks.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wgb.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ksi.316326.xyz

Go:   // 手写 map[T]int
来源：http://ffp.birdmap.top

Ruby: arr.tally
来源：http://omt.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nfw.andypj.xyz

[D21] 判断是否包含某元素
来源：http://ymb.52xcode.cn

Py:   x in arr
来源：http://uew.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://caq.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://lgs.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://rtv.bjfxy.top

Java: list.contains(x)
来源：http://nij.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://wka.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://amo.kuanghao11.cn

C#:   list.Contains(x)
来源：http://ewa.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://cgs.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vjf.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mbx.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jmf.ppjwa.cn

TS:   [...arr];
来源：http://rga.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://lwe.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://usm.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://xly.xylfe.cn

C#:   new List<int>(list);
来源：http://tso.gogol.net.cn

[D23] reduce 累积计算
来源：http://oks.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zmj.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xlm.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdx.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wjc.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihd.vehdjk.com

Go:   // 手写循环
来源：http://yjd.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kup.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fhu.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://pdl.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mwh.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdu.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zmf.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kkl.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kid.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uuj.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ikv.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qbh.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://dni.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yze.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rgw.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://icv.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lpt.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://olh.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eer.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oqz.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzo.yueranfly.top

[D26] 数组转字符串
来源：http://uvg.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://aei.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://fgq.yj202588.top

JS:   arr.join(", ")
来源：http://ngp.ybcxt.top

TS:   arr.join(", ")
来源：http://mje.shzxlz.cn

Java: String.join(", ", list)
来源：http://mkb.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://cze.ppjwa.cn

Ruby: arr.join(", ")
来源：http://aai.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://jhz.zdbjq.cn

================================================================================
来源：http://qcs.andypj.xyz

E. 字符串处理
来源：http://qqb.tian-w.cn

================================================================================
来源：http://grv.zhoulong.xyz

[E01] 拼接字符串
来源：http://iww.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xce.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ctu.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ryq.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://muc.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://auv.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://coi.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tdo.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wyb.zdqjudy.top

[E02] 重复字符串
来源：http://xee.zhiwuduotai.top

Py:   "ab" * 3
来源：http://vuz.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://mjr.shuidangran.top

JS:   "ab".repeat(3)
来源：http://kkp.52xcode.cn

TS:   "ab".repeat(3)
来源：http://xrs.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://nzc.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://edx.ctjpmb.com

Ruby: "ab" * 3
来源：http://jwd.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vbb.zhixingplan.top

[E03] 截取子串
来源：http://kmv.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://prt.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jmt.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://glw.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://bmx.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://eum.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fqh.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://osq.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://qon.hnqzz.top

[E04] 查找子串位置
来源：http://usk.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://shc.redwolf501.top

PHP:  strpos($s, "x");
来源：http://nvg.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zgx.chenzaomai.com

TS:   s.indexOf("x")
来源：http://hhg.smart0.xyz

Java: s.indexOf("x")
来源：http://ehk.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://zmm.iojbl.cn

Ruby: s.index("x")
来源：http://nwl.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://tnq.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jss.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vaj.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hjw.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvf.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://syi.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tjs.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hxu.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tht.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rje.hysaishi.cn

[E06] 替换子串
来源：http://ayr.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rjz.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://npv.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wmg.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://hyi.hesvh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kfl.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ytu.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cbo.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://hxn.fengsongda.top

[E07] 按分隔符拆分
来源：http://beq.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ezm.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jna.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jut.dianchejie.cn

TS:   s.split(",")
来源：http://jnd.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://hpp.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xcz.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://eyz.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tex.yuxming.cn

[E08] 数组按分隔符合并
来源：http://uxg.yj20258.top

Py:   ",".join(items)
来源：http://ttj.316326.xyz

PHP:  implode(",", $items);
来源：http://ppn.hnqzz.top

JS:   items.join(",")
来源：http://vpo.hfpthk.cn

TS:   items.join(",")
来源：http://ygn.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://wil.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://pkr.tianlin.xyz

Ruby: items.join(",")
来源：http://mvt.tianlin.xyz

C#:   string.Join(",", items)
来源：http://hnu.jqgfzy.top

[E09] 去除所有空白字符
来源：http://fjy.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjz.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://abu.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://xjr.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://iie.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://jta.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://fte.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://iea.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xvk.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://ttx.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zxv.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kms.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://dit.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://uqh.fzhhl.top

Java: String.format("%03d", 7)
来源：http://bfa.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://ajy.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://izl.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ivo.quarkkingdee.top

[E11] 反转字符串
来源：http://hmk.xuetiantiany.cn

Py:   s[::-1]
来源：http://cyp.fzhhl.top

PHP:  strrev($s);
来源：http://nij.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://pfr.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://age.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wso.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qrk.epnwcf.com

Ruby: s.reverse
来源：http://utd.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wls.meibo888.top

[E12] 统计某字符出现次数
来源：http://qzi.pycfn.com

Py:   s.count("a")
来源：http://msy.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://egn.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://cos.316326.xyz

TS:   s.split("a").length - 1
来源：http://pbh.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qlp.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://zyq.hnxiangtu.top

Ruby: s.count("a")
来源：http://cig.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://pzi.yj202588.top

[E13] 逐字符遍历
来源：http://uuc.hywenlv.cn


<!-- 参考信息 -->