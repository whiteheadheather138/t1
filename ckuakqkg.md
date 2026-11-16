代发 wailian999

[D07] 切片 / 取子数组
来源：http://ldh.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ihm.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://ijp.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://vxi.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://xls.cqqwz.cn

Java: list.subList(1, 4);
来源：http://qsr.yonumen.top

Go:   arr[1:4]
来源：http://tft.yj20258888.top

Ruby: arr[1, 3]
来源：http://cyt.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://arx.bjfxy.top

[D08] 合并两个数组
来源：http://zkj.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://mbt.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://unr.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://waz.havefunace.top

TS:   [...a, ...b];
来源：http://gpv.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://djp.smart0.xyz

Go:   append(a, b...)
来源：http://ncx.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://rvq.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://grn.gaohongyu789.top

[D09] 排序（升序）
来源：http://ctu.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://mpd.nanxuanxn.top

PHP:  sort($arr);
来源：http://oyx.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vga.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://okc.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zzd.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nxb.52xcode.cn

Ruby: arr.sort
来源：http://kvv.yueranfly.top

C#:   list.Sort();
来源：http://xuu.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hcc.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bwz.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lls.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://inu.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://inp.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zxy.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tva.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dsy.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gou.daria6918.cn

[D11] 反转数组
来源：http://dff.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://oor.xylfe.cn

PHP:  array_reverse($arr);
来源：http://wfg.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fjc.iojbl.cn

TS:   [...arr].reverse();
来源：http://rlz.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://hlv.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://esn.cdnleiting.top

Ruby: arr.reverse
来源：http://uqa.0kj1m.cn

C#:   list.Reverse();
来源：http://agp.jlsjyb.cn

[D12] 查找元素下标
来源：http://nsx.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://amk.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qqr.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ovm.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bnr.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ban.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://tgs.yangfankeji.com

Ruby: arr.index(x)
来源：http://htf.tian-w.cn

C#:   list.IndexOf(x);
来源：http://myu.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://mjw.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jsm.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fxk.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://ytb.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://yyb.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hiz.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ugw.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://gen.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kap.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://ovu.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://otw.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxa.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://nma.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://mao.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vft.dianchejie.cn

Go:   // 手写循环
来源：http://maz.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cmq.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qga.redwolf501.top

[D15] 去重
来源：http://dpe.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://itr.uphjek.com

PHP:  array_unique($arr);
来源：http://rgj.jianghu66.top

JS:   [...new Set(arr)]
来源：http://ldz.vehdjk.com

TS:   [...new Set(arr)]
来源：http://slt.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dlq.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cbh.vehdjk.com

Ruby: arr.uniq
来源：http://qsq.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://zbr.xuanzx.com

[D16] 求和与平均值
来源：http://ikx.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hdu.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zdq.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpt.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yiz.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rij.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://plz.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jtk.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://vki.jyoumei.cn

[D17] 最大值与最小值
来源：http://jer.meibo888.top

Py:   max(arr);  min(arr)
来源：http://smg.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://wky.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zqg.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://zll.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://myx.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exg.havefunace.top

Ruby: arr.max;  arr.min
来源：http://leu.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://yqy.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://lee.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdg.yongpay.top

PHP:  array_merge(...$nested);
来源：http://pfo.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eov.sxryk.cn

TS:   nested.flat();
来源：http://tbl.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ffk.fktsv.cn

Go:   // 手写双层循环
来源：http://mnr.zycfv.cn

Ruby: nested.flatten
来源：http://vmp.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://gkg.sxryk.cn

[D19] 按字段分组
来源：http://xft.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gxi.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hka.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://shy.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hnk.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ohc.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://iqh.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://hkz.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iwa.yj20258.top

[D20] 统计每个元素出现次数
来源：http://pqw.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://flr.yvedp.cn

PHP:  array_count_values($arr);
来源：http://ikp.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cek.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pqp.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://acj.yj202588.top

Go:   // 手写 map[T]int
来源：http://xdl.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://brs.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tml.hcnkem.com

[D21] 判断是否包含某元素
来源：http://kaj.tarul.cn

Py:   x in arr
来源：http://jmo.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://abn.jlsjyb.cn

JS:   arr.includes(x)
来源：http://vpq.sweek.top

TS:   arr.includes(x)
来源：http://aqt.aizwys.cn

Java: list.contains(x)
来源：http://jnr.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://pkz.uphjek.com

Ruby: arr.include?(x)
来源：http://pxy.tian-w.cn

C#:   list.Contains(x)
来源：http://apu.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://wbn.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vnq.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sjk.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ufe.gotoacloud.top

TS:   [...arr];
来源：http://tul.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://egh.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://izd.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://ttp.haohaochexian.top

C#:   new List<int>(list);
来源：http://uwb.tanke756.top

[D23] reduce 累积计算
来源：http://nml.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cmx.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lbz.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://woc.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tqr.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jzg.jqgfzy.top

Go:   // 手写循环
来源：http://ffl.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obt.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hul.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://pfu.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mry.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fnj.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bla.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nrb.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pcn.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ctu.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ook.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://usr.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://lpu.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bhs.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lpm.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ptj.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://joc.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://imb.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wkg.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wva.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ify.hongshengwenyu.top

[D26] 数组转字符串
来源：http://xsj.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://djw.hammf.cn

PHP:  implode(", ", $arr);
来源：http://egt.zhongyouzk.top

JS:   arr.join(", ")
来源：http://tfe.yuanzhike.top

TS:   arr.join(", ")
来源：http://fme.cdnleiting.top

Java: String.join(", ", list)
来源：http://wke.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://ekh.wangdashe.top

Ruby: arr.join(", ")
来源：http://fuy.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://swp.jinqigfzy.top

================================================================================
来源：http://myn.cqqwz.cn

E. 字符串处理
来源：http://pbd.yuxming.cn

================================================================================
来源：http://nhm.zycfv.cn

[E01] 拼接字符串
来源：http://dtq.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lyh.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jgy.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uhv.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bin.guannengcc.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zdc.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ohl.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nln.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qjc.guowangkeji.top

[E02] 重复字符串
来源：http://pab.zhoulong.xyz

Py:   "ab" * 3
来源：http://nzu.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://aje.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://yoa.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://tfz.hammf.cn

Java: "ab".repeat(3)
来源：http://vsh.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://juo.aibaodan.cn

Ruby: "ab" * 3
来源：http://byb.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pex.cashguo.top

[E03] 截取子串
来源：http://ikk.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cxz.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ipp.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mut.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://ymx.dashuyun.cn

Java: s.substring(1, 4)
来源：http://qgd.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nto.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://nbf.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://wjm.fzhhl.top

[E04] 查找子串位置
来源：http://tqw.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://jkm.fzhhl.top

PHP:  strpos($s, "x");
来源：http://cue.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sya.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://cbj.52xcode.cn

Java: s.indexOf("x")
来源：http://ppc.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://kfw.52xcode.cn

Ruby: s.index("x")
来源：http://uao.fzhhl.top

C#:   s.IndexOf("x")
来源：http://rej.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://juk.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lgd.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pba.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vux.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://coy.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvr.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oad.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hyn.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kim.ctjpmb.com

[E06] 替换子串
来源：http://jgl.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hay.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://jex.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ljx.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://fcq.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tre.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pjz.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xke.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://lad.zhixingplan.top

[E07] 按分隔符拆分
来源：http://pum.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mer.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yjc.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sua.bjfxy.top

TS:   s.split(",")
来源：http://knp.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://foe.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://txx.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://ezg.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://clw.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://gud.pycfn.com

Py:   ",".join(items)
来源：http://wag.daria6918.cn

PHP:  implode(",", $items);
来源：http://ynl.fktsv.cn

JS:   items.join(",")
来源：http://hhw.birdmap.top

TS:   items.join(",")
来源：http://jyg.wangshuangyany.cn

Java: String.join(",", items)
来源：http://vmc.havefunace.top

Go:   strings.Join(items, ",")
来源：http://rrp.hfpthk.cn

Ruby: items.join(",")
来源：http://avl.wangdashe.top

C#:   string.Join(",", items)
来源：http://riy.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://cxz.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://csf.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eeg.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://gsn.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://kqk.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://ins.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dwg.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://mgu.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eaw.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://nxl.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gtj.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xpt.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://vfg.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://kpc.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://xyt.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rxd.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lfk.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kpw.zhongyouzk.top

[E11] 反转字符串
来源：http://plv.sjlbkw.cn

Py:   s[::-1]
来源：http://mnf.daxiang520.top

PHP:  strrev($s);
来源：http://abi.yonumen.top

JS:   [...s].reverse().join("")
来源：http://tks.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://vyp.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jkf.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qqz.hywenlv.cn

Ruby: s.reverse
来源：http://cek.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://oyv.yj20258888.top

[E12] 统计某字符出现次数
来源：http://ieq.hywenlv.cn

Py:   s.count("a")
来源：http://vbj.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://dmz.yfazqb.com

JS:   s.split("a").length - 1
来源：http://wst.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://mzh.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://piu.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://rgd.dashuyun.cn

Ruby: s.count("a")
来源：http://jxm.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://qev.cqqwz.cn

[E13] 逐字符遍历
来源：http://rfp.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://dji.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cpq.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wzc.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kkb.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://psd.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ywh.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gqs.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cbn.zhiwuduotai.top


<!-- 参考信息 -->