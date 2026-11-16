代发 wailian999

Py:   len(arr)
来源：http://hou.vqdsnc.cn

PHP:  count($arr);
来源：http://avn.meibo888.top

JS:   arr.length
来源：http://vqi.guannengcc.top

TS:   arr.length
来源：http://mqq.chenlongwang.top

Java: list.size();
来源：http://une.tian-w.cn

Go:   len(arr)
来源：http://bzc.smart0.xyz

Ruby: arr.length; arr.size
来源：http://rmj.zhoulong.xyz

C#:   list.Count;
来源：http://riu.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://qup.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vxw.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tld.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://koo.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://owk.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://wil.0kj1m.cn

Go:   arr[1:4]
来源：http://dpp.zdbjq.cn

Ruby: arr[1, 3]
来源：http://cst.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://pvs.jinqigfzy.top

[D08] 合并两个数组
来源：http://gjy.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://qwc.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://scl.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://omy.sufxvd.cn

TS:   [...a, ...b];
来源：http://axo.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xss.hnqzz.top

Go:   append(a, b...)
来源：http://jar.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://mpr.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://sxs.jianghu66.top

[D09] 排序（升序）
来源：http://xwa.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://nfm.fktsv.cn

PHP:  sort($arr);
来源：http://ows.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xqs.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xwf.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://xja.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://paf.jqgfzy.top

Ruby: arr.sort
来源：http://cuw.yanxiufei.cn

C#:   list.Sort();
来源：http://buj.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://qon.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zsg.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zlq.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymd.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bum.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pks.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mhq.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pke.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://siz.hnqzz.top

[D11] 反转数组
来源：http://dhc.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jhp.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://zhh.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ari.xuanzx.com

TS:   [...arr].reverse();
来源：http://bbe.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://dvr.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://tui.zdqjudy.top

Ruby: arr.reverse
来源：http://cbf.nanxinkj.top

C#:   list.Reverse();
来源：http://pkk.hcnkem.com

[D12] 查找元素下标
来源：http://hbn.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://nea.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dgm.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qmh.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lkk.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uaz.havefunace.top

Go:   slices.Index(arr, x)
来源：http://ohm.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://vjt.daxiang520.top

C#:   list.IndexOf(x);
来源：http://jth.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://idu.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwh.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hqu.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://nqj.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://arr.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qzs.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kwl.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rro.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rbc.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://ore.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://clo.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ere.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://nec.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://gwx.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://not.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://sju.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://hhu.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yij.jinqigufen.top

[D15] 去重
来源：http://mdi.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lzn.guowangkeji.top

PHP:  array_unique($arr);
来源：http://vei.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://bfb.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://uhw.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://frk.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://let.tianlin.xyz

Ruby: arr.uniq
来源：http://jmi.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://sqk.mhx1999.top

[D16] 求和与平均值
来源：http://oho.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jwi.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lcp.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pzv.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zox.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xvj.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://khj.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qtn.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://txu.hcnkem.com

[D17] 最大值与最小值
来源：http://ivz.yj20258.top

Py:   max(arr);  min(arr)
来源：http://kum.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://crw.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jut.ybcxt.top

TS:   Math.max(...arr);
来源：http://tnx.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kwn.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nnp.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://awg.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://apx.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://yaf.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vfb.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://aws.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lah.hywenlv.cn

TS:   nested.flat();
来源：http://lua.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://btd.tanke756.top

Go:   // 手写双层循环
来源：http://nab.quarkkingdee.top

Ruby: nested.flatten
来源：http://cdn.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bnl.zhoulong.xyz

[D19] 按字段分组
来源：http://omp.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://adh.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ulp.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pqm.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tgd.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://avv.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://mlu.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ynr.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jhe.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://hjm.daxiang520.top

Py:   Counter(arr)
来源：http://mhz.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://irt.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qas.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cdp.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zvi.yueranfly.top

Go:   // 手写 map[T]int
来源：http://hyo.wangdashe.top

Ruby: arr.tally
来源：http://xax.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tbh.smart0.xyz

[D21] 判断是否包含某元素
来源：http://vrd.hongshengwenyu.top

Py:   x in arr
来源：http://hyd.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://xol.yongpay.top

JS:   arr.includes(x)
来源：http://sqi.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://jhw.tian-w.cn

Java: list.contains(x)
来源：http://poo.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://skg.c1oappe.top

Ruby: arr.include?(x)
来源：http://rvi.dianchejie.cn

C#:   list.Contains(x)
来源：http://kdh.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://lsx.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aww.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qlp.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hcb.fanxiaobao.xyz

TS:   [...arr];
来源：http://klk.fzhhl.top

Java: new ArrayList<>(list);
来源：http://ign.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://ddm.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://bko.nanxinkj.top

C#:   new List<int>(list);
来源：http://jro.yuxming.cn

[D23] reduce 累积计算
来源：http://lei.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pve.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wlt.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bcj.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ylg.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://djw.xylfe.cn

Go:   // 手写循环
来源：http://xtx.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rfu.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cfg.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://rkt.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zed.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lfz.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://axc.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ntm.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kaw.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://frh.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://alt.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://diu.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://pvr.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mej.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://meq.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dll.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tqv.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://frh.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mvt.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ddj.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uoh.jinqigufen.top

[D26] 数组转字符串
来源：http://osa.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://qkc.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://ioi.mhx1999.top

JS:   arr.join(", ")
来源：http://qke.hnxiangtu.top

TS:   arr.join(", ")
来源：http://gsf.guannengcc.top

Java: String.join(", ", list)
来源：http://ntr.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://ttf.yangfankeji.com

Ruby: arr.join(", ")
来源：http://wab.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://cis.zycfv.cn

================================================================================
来源：http://ksx.yanxiufei.cn

E. 字符串处理
来源：http://wlu.sysykeji.top

================================================================================
来源：http://pwp.fktsv.cn

[E01] 拼接字符串
来源：http://chg.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xsa.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iod.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofx.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://umt.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gdb.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oer.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ndh.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://caw.sysykeji.top

[E02] 重复字符串
来源：http://zhq.uphjek.com

Py:   "ab" * 3
来源：http://ifo.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://fqx.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://guv.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://cck.jqgfzy.top

Java: "ab".repeat(3)
来源：http://tnt.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://wxp.kuanghao11.cn

Ruby: "ab" * 3
来源：http://xxr.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hch.shangyingyoupin.top

[E03] 截取子串
来源：http://qje.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://emt.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wsd.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lgh.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://cja.bjfxy.top

Java: s.substring(1, 4)
来源：http://xzf.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://akk.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://vem.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://tye.ppjwa.cn

[E04] 查找子串位置
来源：http://kut.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://diy.ybcxt.top

PHP:  strpos($s, "x");
来源：http://pnc.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iab.jiagoushi.top

TS:   s.indexOf("x")
来源：http://asi.jqgufenzy.top

Java: s.indexOf("x")
来源：http://fji.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://ntb.iojbl.cn

Ruby: s.index("x")
来源：http://eql.yfazqb.com

C#:   s.IndexOf("x")
来源：http://klz.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://czy.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cxp.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qdy.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxm.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://qdz.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qhl.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zkf.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wrp.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wji.zdbjq.cn

[E06] 替换子串
来源：http://rkk.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vzf.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://tzp.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mhg.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://pto.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cki.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sul.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eua.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://vhn.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://hqu.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nra.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvw.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gfi.ivvv.top

TS:   s.split(",")
来源：http://uuv.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://uqt.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://idt.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://iku.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bef.bbcook.cn

[E08] 数组按分隔符合并
来源：http://jaw.chenzaomai.com

Py:   ",".join(items)
来源：http://fkx.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://kwr.fanxiaobao.xyz

JS:   items.join(",")
来源：http://acf.yonumen.top

TS:   items.join(",")
来源：http://yna.chenjidiqi.icu

Java: String.join(",", items)
来源：http://epk.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://qcr.xziqi.cn

Ruby: items.join(",")
来源：http://got.ydzc1.top

C#:   string.Join(",", items)
来源：http://ngr.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://exj.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tog.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qgk.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://mws.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://blx.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://hif.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pci.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hlq.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jmg.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://lai.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cbo.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zir.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://psn.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://rme.tian-w.cn

Java: String.format("%03d", 7)
来源：http://ptg.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rhf.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xbk.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhe.fehbvm.com

[E11] 反转字符串
来源：http://lbg.0kj1m.cn

Py:   s[::-1]
来源：http://ytw.52xcode.cn

PHP:  strrev($s);
来源：http://pwl.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://ale.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://egf.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ujw.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://iah.svipenyu.cn

Ruby: s.reverse
来源：http://ajh.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://xyq.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://zvd.jqgufenzy.top

Py:   s.count("a")
来源：http://lrz.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://jaj.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://jxe.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://hvy.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rcx.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://gar.hammf.cn

Ruby: s.count("a")
来源：http://axg.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://rtv.vqdsnc.cn

[E13] 逐字符遍历
来源：http://tri.nanxinkj.top


<!-- 参考信息 -->