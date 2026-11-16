代发 wailian999

[D07] 切片 / 取子数组
来源：http://dqq.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rcl.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://gbo.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://nnb.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://xjw.jinqigufen.top

Java: list.subList(1, 4);
来源：http://myj.vqdsnc.cn

Go:   arr[1:4]
来源：http://zvi.fzhhl.top

Ruby: arr[1, 3]
来源：http://qya.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://aqr.jinqigfzy.top

[D08] 合并两个数组
来源：http://ewq.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://lyj.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://ezm.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://htu.xuanzx.com

TS:   [...a, ...b];
来源：http://ihd.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hoi.fehbvm.com

Go:   append(a, b...)
来源：http://lph.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://fwq.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://jqu.wangdashe.top

[D09] 排序（升序）
来源：http://vai.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://jup.zdbjq.cn

PHP:  sort($arr);
来源：http://onp.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wzr.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cfi.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wcu.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://olo.zhixingplan.top

Ruby: arr.sort
来源：http://izt.ehwqpu.com

C#:   list.Sort();
来源：http://mrv.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lba.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bcg.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fig.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://skx.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xzl.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zqg.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://csg.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lwt.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xyg.zhoulong.xyz

[D11] 反转数组
来源：http://vdw.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://axr.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://thj.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xzu.ivvv.top

TS:   [...arr].reverse();
来源：http://khj.cheryme.top

Java: Collections.reverse(list);
来源：http://jkx.yongpay.top

Go:   slices.Reverse(arr)
来源：http://iqk.jqgufenzy.top

Ruby: arr.reverse
来源：http://wzv.dashuyun.cn

C#:   list.Reverse();
来源：http://wii.zdbjq.cn

[D12] 查找元素下标
来源：http://fat.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://pmq.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ssb.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vpg.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ubl.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vnq.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://sel.zdqjudy.top

Ruby: arr.index(x)
来源：http://aqu.yvedp.cn

C#:   list.IndexOf(x);
来源：http://hpk.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://vgi.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hhh.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qfk.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://qmg.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://lci.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fcg.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vvc.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://efa.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://goq.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://ckd.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dwf.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://klq.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://hmj.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://ajn.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://obm.daria6918.cn

Go:   // 手写循环
来源：http://wun.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://svw.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jes.yj20258.top

[D15] 去重
来源：http://emo.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kwq.c1oappe.top

PHP:  array_unique($arr);
来源：http://vzo.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://ivm.bbcook.cn

TS:   [...new Set(arr)]
来源：http://gio.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://txx.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qtj.daxiang520.top

Ruby: arr.uniq
来源：http://esf.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://aer.ctjpmb.com

[D16] 求和与平均值
来源：http://wsg.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yuz.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jbf.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdj.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wyj.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wmd.havefunace.top

Go:   // 手写循环累加
来源：http://cwt.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://geo.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://xux.yonumen.top

[D17] 最大值与最小值
来源：http://hcy.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://scd.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://jyk.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tww.ppjwa.cn

TS:   Math.max(...arr);
来源：http://iwr.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bpg.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ckn.meibo888.top

Ruby: arr.max;  arr.min
来源：http://agf.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://qza.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://wrh.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zcp.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://hwf.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ovc.zhengqikj.top

TS:   nested.flat();
来源：http://caw.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ksj.zhongyouzk.top

Go:   // 手写双层循环
来源：http://cnn.shuidangran.top

Ruby: nested.flatten
来源：http://ifi.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mxc.andypj.xyz

[D19] 按字段分组
来源：http://eng.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mor.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hag.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://puf.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mai.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vgc.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://ozc.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://itk.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uid.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://juc.hammf.cn

Py:   Counter(arr)
来源：http://nud.bbcook.cn

PHP:  array_count_values($arr);
来源：http://cgv.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqr.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://apr.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://biy.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://bds.yvedp.cn

Ruby: arr.tally
来源：http://wol.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gps.xylfe.cn

[D21] 判断是否包含某元素
来源：http://ydu.hcnkem.com

Py:   x in arr
来源：http://npl.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://zra.yfazqb.com

JS:   arr.includes(x)
来源：http://eex.zdqjudy.top

TS:   arr.includes(x)
来源：http://yqo.yj202588.top

Java: list.contains(x)
来源：http://dcy.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://sex.ivvv.top

Ruby: arr.include?(x)
来源：http://vzb.guannengcc.top

C#:   list.Contains(x)
来源：http://blq.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://wuk.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ccj.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zjz.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fcv.pengpengdd.cyou

TS:   [...arr];
来源：http://uwz.cashguo.top

Java: new ArrayList<>(list);
来源：http://gjz.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://mga.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://bhf.nanxinkj.top

C#:   new List<int>(list);
来源：http://fgb.cucudq.cn

[D23] reduce 累积计算
来源：http://kse.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://isn.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qav.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozk.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://utq.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uev.xylfe.cn

Go:   // 手写循环
来源：http://pbx.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kqe.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wwg.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://rvs.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rtd.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hna.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eld.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mxz.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xdq.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ahy.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ddc.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yze.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://fgk.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gqb.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bgp.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://flh.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sxs.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qtb.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://osn.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xvo.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uid.havefunace.top

[D26] 数组转字符串
来源：http://csa.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://eix.hammf.cn

PHP:  implode(", ", $arr);
来源：http://fwo.hnqzz.top

JS:   arr.join(", ")
来源：http://hlg.sufxvd.cn

TS:   arr.join(", ")
来源：http://qeu.yj20258.top

Java: String.join(", ", list)
来源：http://dut.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://ncp.xziqi.cn

Ruby: arr.join(", ")
来源：http://dje.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://iir.zdqjudy.top

================================================================================
来源：http://gzx.yongpay.top

E. 字符串处理
来源：http://bds.hywenlv.cn

================================================================================
来源：http://uqo.ybcxt.top

[E01] 拼接字符串
来源：http://odl.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vjl.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ywp.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hac.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fdr.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pbg.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rmt.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://axw.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bsc.aizwys.cn

[E02] 重复字符串
来源：http://sej.nanxuanxn.top

Py:   "ab" * 3
来源：http://cif.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://mge.yueranfly.top

JS:   "ab".repeat(3)
来源：http://qdr.cashguo.top

TS:   "ab".repeat(3)
来源：http://elo.bjfxy.top

Java: "ab".repeat(3)
来源：http://bfw.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://fdk.vqdsnc.cn

Ruby: "ab" * 3
来源：http://ons.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pmz.aizwys.cn

[E03] 截取子串
来源：http://ivx.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aea.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vjn.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oqn.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://ygc.hysaishi.cn

Java: s.substring(1, 4)
来源：http://lvn.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wwx.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rbd.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://hpm.yangfankeji.com

[E04] 查找子串位置
来源：http://kjn.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://zrx.havefunace.top

PHP:  strpos($s, "x");
来源：http://zzv.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vbd.c1oappe.top

TS:   s.indexOf("x")
来源：http://oac.snrcjt.cn

Java: s.indexOf("x")
来源：http://lcg.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://bzp.jqgfzy.top

Ruby: s.index("x")
来源：http://qlx.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://xxs.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://pph.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hhs.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mng.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bvx.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lfz.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qwc.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gvw.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gzq.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://umb.chenjidiqi.icu

[E06] 替换子串
来源：http://oxv.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ley.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://gik.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rhi.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://vdx.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bzn.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xqx.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ozc.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://apv.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://lqm.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bfh.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uff.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rqf.zycfv.cn

TS:   s.split(",")
来源：http://aae.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://fjw.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tqr.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://zji.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dhw.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://rjo.tarul.cn

Py:   ",".join(items)
来源：http://bty.hysaishi.cn

PHP:  implode(",", $items);
来源：http://gzl.xuanzx.com

JS:   items.join(",")
来源：http://fup.sysykeji.top

TS:   items.join(",")
来源：http://skg.nwbrower.top

Java: String.join(",", items)
来源：http://lrf.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://lmt.zdqjudy.top

Ruby: items.join(",")
来源：http://qwa.yuanzhike.top

C#:   string.Join(",", items)
来源：http://rxe.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://lse.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tzn.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lir.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://lac.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://wai.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://vpr.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kmy.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://alf.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cva.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://uyd.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dau.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fwc.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://alq.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://lwu.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://wqm.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hsm.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vtx.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ibz.wangshuangyany.cn

[E11] 反转字符串
来源：http://amr.shanyushiyangtech.top

Py:   s[::-1]
来源：http://zqp.cheryme.top

PHP:  strrev($s);
来源：http://qkd.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://psq.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://kcu.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pte.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gmx.vehdjk.com

Ruby: s.reverse
来源：http://hlr.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://tqc.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://oal.zhoulong.xyz

Py:   s.count("a")
来源：http://fmo.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://yma.cashguo.top

JS:   s.split("a").length - 1
来源：http://let.cucudq.cn

TS:   s.split("a").length - 1
来源：http://nrw.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uco.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://ltj.tian-w.cn

Ruby: s.count("a")
来源：http://szs.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://lco.sufxvd.cn

[E13] 逐字符遍历
来源：http://fyr.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://hyr.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jnu.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xev.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mdw.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qmc.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bqc.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hje.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://drt.zdbjq.cn


<!-- 参考信息 -->