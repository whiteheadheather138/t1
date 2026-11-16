代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://atk.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hmi.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://nrs.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://vjt.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://pju.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ogc.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gdm.yueranfly.top

[D06] 数组长度
来源：http://mfw.sjlbkw.cn

Py:   len(arr)
来源：http://oei.sysykeji.top

PHP:  count($arr);
来源：http://jcj.bbcook.cn

JS:   arr.length
来源：http://dcr.gogol.net.cn

TS:   arr.length
来源：http://wuf.cqqwz.cn

Java: list.size();
来源：http://zit.uphjek.com

Go:   len(arr)
来源：http://qiw.birdmap.top

Ruby: arr.length; arr.size
来源：http://vxy.chenjidiqi.icu

C#:   list.Count;
来源：http://rjm.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://yby.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jdb.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://ine.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://gas.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://dev.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://qcs.aizwys.cn

Go:   arr[1:4]
来源：http://vdb.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://epw.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://eyw.hywenlv.cn

[D08] 合并两个数组
来源：http://bsb.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://hhw.ivvv.top

PHP:  array_merge($a, $b);
来源：http://iib.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fsj.shuidangran.top

TS:   [...a, ...b];
来源：http://zvh.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://itd.c1oappe.top

Go:   append(a, b...)
来源：http://qtq.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://lcy.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://ess.yuxming.cn

[D09] 排序（升序）
来源：http://cbf.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://ipk.sufxvd.cn

PHP:  sort($arr);
来源：http://owx.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lhb.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://dis.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kri.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bsw.cqqwz.cn

Ruby: arr.sort
来源：http://vov.sjlbkw.cn

C#:   list.Sort();
来源：http://ytd.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://yus.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpd.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://exr.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ccp.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oks.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oar.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bhq.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://msu.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qnd.vehdjk.com

[D11] 反转数组
来源：http://utw.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://umz.ivvv.top

PHP:  array_reverse($arr);
来源：http://xfb.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://boy.ivvv.top

TS:   [...arr].reverse();
来源：http://pgv.gogol.net.cn

Java: Collections.reverse(list);
来源：http://weg.tarul.cn

Go:   slices.Reverse(arr)
来源：http://xft.jqgfzy.top

Ruby: arr.reverse
来源：http://jjc.aibaodan.cn

C#:   list.Reverse();
来源：http://biv.0kj1m.cn

[D12] 查找元素下标
来源：http://cpy.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://qgk.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jst.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mok.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igj.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jpt.316326.xyz

Go:   slices.Index(arr, x)
来源：http://mdg.jiagoushi.top

Ruby: arr.index(x)
来源：http://msq.cashguo.top

C#:   list.IndexOf(x);
来源：http://vxc.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://fld.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dzu.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nfv.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://jym.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://hhe.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lez.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tfc.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://xar.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qkm.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://pob.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eyh.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wiy.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://cpn.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://mip.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lrz.jlsjyb.cn

Go:   // 手写循环
来源：http://nfu.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://xcn.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wni.cashguo.top

[D15] 去重
来源：http://kzg.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vak.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://gxs.yj20258.top

JS:   [...new Set(arr)]
来源：http://woa.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://pta.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nts.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kep.andypj.xyz

Ruby: arr.uniq
来源：http://zfh.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://lto.yuanzhike.top

[D16] 求和与平均值
来源：http://mwy.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fjp.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vpy.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eov.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ymz.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ptw.gogol.net.cn

Go:   // 手写循环累加
来源：http://bch.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jhx.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://ntc.vqdsnc.cn

[D17] 最大值与最小值
来源：http://fza.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://phn.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://ofv.sysykeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kin.sufxvd.cn

TS:   Math.max(...arr);
来源：http://jlf.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://slj.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ndd.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://sdx.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://rov.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://mpl.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xzd.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://koa.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://asw.yongpay.top

TS:   nested.flat();
来源：http://wwp.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zja.redwolf501.top

Go:   // 手写双层循环
来源：http://hsf.9152youxi.cn

Ruby: nested.flatten
来源：http://smc.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jeb.yfazqb.com

[D19] 按字段分组
来源：http://tsx.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edg.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jpj.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://isa.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://joy.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nsz.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://qrr.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tlt.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://esi.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://sna.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://lqz.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://dcs.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zuf.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nhd.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sbu.zycfv.cn

Go:   // 手写 map[T]int
来源：http://wog.cdnleiting.top

Ruby: arr.tally
来源：http://mnw.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cmk.tian-w.cn

[D21] 判断是否包含某元素
来源：http://ani.52xcode.cn

Py:   x in arr
来源：http://xeu.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://kgz.jinqigufen.top

JS:   arr.includes(x)
来源：http://non.cashguo.top

TS:   arr.includes(x)
来源：http://wap.jinghuilouyu.cn

Java: list.contains(x)
来源：http://mnw.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://vhk.zhixingplan.top

Ruby: arr.include?(x)
来源：http://lkg.tian-w.cn

C#:   list.Contains(x)
来源：http://lfu.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://evf.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tau.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ygc.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xra.ivvv.top

TS:   [...arr];
来源：http://iel.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://vih.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://uqf.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://int.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://uvd.fzhhl.top

[D23] reduce 累积计算
来源：http://uog.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rix.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://riw.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://elg.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gsv.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxd.iojbl.cn

Go:   // 手写循环
来源：http://iaz.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dwh.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zuy.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://jup.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hvh.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sqt.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rxo.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wvn.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://klf.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rok.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rph.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hjc.pycfn.com

[D25] Set 集合去重与交并差
来源：http://zbj.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://til.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://haq.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iiw.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iar.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cnp.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://obd.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uur.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zkt.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://raz.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://nao.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://uyx.sweek.top

JS:   arr.join(", ")
来源：http://ijo.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://cdc.gzhubu.top

Java: String.join(", ", list)
来源：http://wus.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://nus.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://obm.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://acu.gogol.net.cn

================================================================================
来源：http://noe.9152youxi.cn

E. 字符串处理
来源：http://sof.sjlbkw.cn

================================================================================
来源：http://bkt.andypj.xyz

[E01] 拼接字符串
来源：http://qha.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eka.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://amh.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kth.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tfr.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://swl.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lvk.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vlb.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rfv.wangshuangyany.cn

[E02] 重复字符串
来源：http://fha.gogol.net.cn

Py:   "ab" * 3
来源：http://juy.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://clo.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://btd.wangdashe.top

TS:   "ab".repeat(3)
来源：http://itd.hfpthk.cn

Java: "ab".repeat(3)
来源：http://ypn.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://xsq.jlsjyb.cn

Ruby: "ab" * 3
来源：http://wdk.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kty.cqqwz.cn

[E03] 截取子串
来源：http://dqd.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://avo.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mjc.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://elb.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://xro.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://dlg.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yef.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yvl.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://kaw.meibo888.top

[E04] 查找子串位置
来源：http://loa.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://cgm.xuetiantiany.cn

PHP:  strpos($s, "x");
来源：http://jof.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://inl.cheryme.top

TS:   s.indexOf("x")
来源：http://qen.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://jeu.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://mnw.ydzc1.top

Ruby: s.index("x")
来源：http://jnp.pycfn.com

C#:   s.IndexOf("x")
来源：http://zoa.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://szo.sufxvd.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sdg.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vcq.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cjy.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pgv.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gns.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xvn.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zjr.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lhy.zdqjudy.top

[E06] 替换子串
来源：http://fah.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://heu.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://kat.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rjs.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://lxn.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wti.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bcs.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ayb.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://svo.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://red.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vmi.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hpx.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ibx.vqdsnc.cn

TS:   s.split(",")
来源：http://iyo.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://gsa.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oox.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://pcm.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxc.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://job.jlsjyb.cn

Py:   ",".join(items)
来源：http://bjj.yvedp.cn

PHP:  implode(",", $items);
来源：http://vrh.guowangkeji.top

JS:   items.join(",")
来源：http://vqn.guowangkeji.top

TS:   items.join(",")
来源：http://oyo.jyoumei.cn

Java: String.join(",", items)
来源：http://opm.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://ewo.tian-w.cn

Ruby: items.join(",")
来源：http://dsj.cheryme.top

C#:   string.Join(",", items)
来源：http://aje.yueranfly.top

[E09] 去除所有空白字符
来源：http://tog.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yok.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oer.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://ebv.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://mip.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://xdg.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sbx.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://mqd.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mvk.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://lcw.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oqg.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hpw.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://uhe.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://mrq.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://jfa.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zut.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxx.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bie.bjfxy.top

[E11] 反转字符串
来源：http://caw.ppjwa.cn

Py:   s[::-1]
来源：http://vcq.yj20258.top

PHP:  strrev($s);
来源：http://tft.ivvv.top

JS:   [...s].reverse().join("")
来源：http://tzw.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://vwv.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://asi.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ose.chenzaomai.com

Ruby: s.reverse
来源：http://jqt.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://zok.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://irv.birdmap.top

Py:   s.count("a")
来源：http://iet.dianchejie.cn


<!-- 参考信息 -->