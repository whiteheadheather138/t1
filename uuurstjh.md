代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://odq.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://bat.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://npe.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nyn.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pwb.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sbt.c1oappe.top

[D05] 访问与修改元素
来源：http://npj.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qkx.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ehd.jinqigufen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://abp.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://gwf.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://oho.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://ghy.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oni.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://doi.epnwcf.com

[D06] 数组长度
来源：http://ulh.smart0.xyz

Py:   len(arr)
来源：http://vro.pengpengdd.cyou

PHP:  count($arr);
来源：http://oro.zycfv.cn

JS:   arr.length
来源：http://pis.birdmap.top

TS:   arr.length
来源：http://tlx.redwolf501.top

Java: list.size();
来源：http://ydo.zhixingplan.top

Go:   len(arr)
来源：http://txy.cashguo.top

Ruby: arr.length; arr.size
来源：http://krf.hnxiangtu.top

C#:   list.Count;
来源：http://oyw.xylfe.cn

[D07] 切片 / 取子数组
来源：http://dbq.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ezg.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hds.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://jlz.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://lyl.fktsv.cn

Java: list.subList(1, 4);
来源：http://gnj.ppjwa.cn

Go:   arr[1:4]
来源：http://mij.hnqzz.top

Ruby: arr[1, 3]
来源：http://kbh.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://gyy.jqgfzy.top

[D08] 合并两个数组
来源：http://qwr.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://itd.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://qrw.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://llm.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://vnp.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tfo.guowangkeji.top

Go:   append(a, b...)
来源：http://xsd.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://hoc.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://enp.haohaochexian.top

[D09] 排序（升序）
来源：http://nms.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://yhg.cqqwz.cn

PHP:  sort($arr);
来源：http://kzp.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mzq.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://umn.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rdr.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wfc.aizwys.cn

Ruby: arr.sort
来源：http://dsz.yueranfly.top

C#:   list.Sort();
来源：http://gde.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wgf.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hsh.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mdv.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ecx.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gdl.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxk.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lxg.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mnk.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ave.ywan-chungtsiang.top

[D11] 反转数组
来源：http://wuw.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://udh.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://smy.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://par.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://dmr.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://eac.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://akg.c1oappe.top

Ruby: arr.reverse
来源：http://dgy.zdbjq.cn

C#:   list.Reverse();
来源：http://gqc.wangshuangyany.cn

[D12] 查找元素下标
来源：http://zax.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://gvo.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gnu.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pyj.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gwu.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bjz.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://elh.hywenlv.cn

Ruby: arr.index(x)
来源：http://pwd.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://hlz.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://nfq.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cne.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cef.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://ljr.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://abi.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jkg.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://phr.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nzc.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oeb.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://axi.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kdz.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dme.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://gox.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://mlk.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://utg.hnqzz.top

Go:   // 手写循环
来源：http://mez.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://snd.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://sjs.epnwcf.com

[D15] 去重
来源：http://quo.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pii.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://alf.tian-w.cn

JS:   [...new Set(arr)]
来源：http://ved.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://erm.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jjx.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://dko.sweek.top

Ruby: arr.uniq
来源：http://tvs.yongpay.top

C#:   list.Distinct().ToList()
来源：http://qwk.zhijiandao.cn

[D16] 求和与平均值
来源：http://fht.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fut.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hsy.jinqigfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qbc.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://krp.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://isv.svipenyu.cn

Go:   // 手写循环累加
来源：http://fzg.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lpg.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://kmg.sysykeji.top

[D17] 最大值与最小值
来源：http://zzi.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://tqg.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://vjx.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dpr.epnwcf.com

TS:   Math.max(...arr);
来源：http://kff.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iwe.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nen.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://gsg.sweek.top

C#:   list.Max();  list.Min()
来源：http://nhp.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://tgt.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kkf.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://fke.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tkd.hnqzz.top

TS:   nested.flat();
来源：http://eyd.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zwz.yvedp.cn

Go:   // 手写双层循环
来源：http://ljn.xylfe.cn

Ruby: nested.flatten
来源：http://cri.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ccd.tarul.cn

[D19] 按字段分组
来源：http://pvd.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bil.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jxh.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nry.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wqg.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fiy.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://lca.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://txf.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gpj.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://txa.svipenyu.cn

Py:   Counter(arr)
来源：http://igv.aizwys.cn

PHP:  array_count_values($arr);
来源：http://dws.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rpp.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wrd.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hbh.yuxming.cn

Go:   // 手写 map[T]int
来源：http://ido.pengpengdd.cyou

Ruby: arr.tally
来源：http://duc.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vav.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://viz.quarkkingdee.top

Py:   x in arr
来源：http://bed.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://vze.jlsjyb.cn

JS:   arr.includes(x)
来源：http://kty.ybcxt.top

TS:   arr.includes(x)
来源：http://jdw.smart0.xyz

Java: list.contains(x)
来源：http://orb.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://aqk.jyoumei.cn

Ruby: arr.include?(x)
来源：http://fbo.zhongyouzk.top

C#:   list.Contains(x)
来源：http://ubp.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://ggj.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://akm.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qip.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://acs.birdmap.top

TS:   [...arr];
来源：http://ggq.yj20258888.top

Java: new ArrayList<>(list);
来源：http://wwx.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vji.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://qvd.zhixingplan.top

C#:   new List<int>(list);
来源：http://jge.vehdjk.com

[D23] reduce 累积计算
来源：http://rou.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zhy.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pwa.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shq.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfs.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ado.ehwqpu.com

Go:   // 手写循环
来源：http://fhb.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kds.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blt.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://pfj.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zlv.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bhg.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ihc.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oln.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iyd.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lgt.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zlp.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vjf.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://tlt.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zax.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cyt.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fox.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ycp.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lyu.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ozr.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jdg.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jww.xinyue.icu

[D26] 数组转字符串
来源：http://tbx.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://zrm.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://pok.gotoacloud.top

JS:   arr.join(", ")
来源：http://uox.gotoacloud.top

TS:   arr.join(", ")
来源：http://rkp.jlsjyb.cn

Java: String.join(", ", list)
来源：http://uyu.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://ilb.dianchejie.cn

Ruby: arr.join(", ")
来源：http://mrk.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://sxz.gzhubu.top

================================================================================
来源：http://gpy.quarkkingdee.top

E. 字符串处理
来源：http://kbn.kuanghao11.cn

================================================================================
来源：http://geo.fengsongda.top

[E01] 拼接字符串
来源：http://gac.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qde.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcm.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aul.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qkw.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rae.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://niw.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tpq.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tbu.epnwcf.com

[E02] 重复字符串
来源：http://pyx.9152youxi.cn

Py:   "ab" * 3
来源：http://paw.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://tim.yj20258.top

JS:   "ab".repeat(3)
来源：http://bbb.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://txd.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://hmk.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://owu.sufxvd.cn

Ruby: "ab" * 3
来源：http://vsa.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://izt.iojbl.cn

[E03] 截取子串
来源：http://jyi.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://prc.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tce.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qoq.yuxming.cn

TS:   s.slice(1, 4)
来源：http://hdg.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://pvv.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qst.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lib.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://lqe.zhiwuduotai.top

[E04] 查找子串位置
来源：http://wuf.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://biu.jianghu66.top

PHP:  strpos($s, "x");
来源：http://zbn.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kze.yangfankeji.com

TS:   s.indexOf("x")
来源：http://icq.zdbjq.cn

Java: s.indexOf("x")
来源：http://cen.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://uhv.sjlbkw.cn

Ruby: s.index("x")
来源：http://sjj.wangdashe.top

C#:   s.IndexOf("x")
来源：http://nms.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sis.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tfb.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://twn.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ywr.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fjj.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://get.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pbn.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bzc.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ulq.9152youxi.cn

[E06] 替换子串
来源：http://sir.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vrp.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://gsw.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ibk.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://tmt.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpx.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ins.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wbk.316326.xyz

C#:   s.Replace("a", "b")
来源：http://kwv.hammf.cn

[E07] 按分隔符拆分
来源：http://zvk.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kyl.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ris.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://esp.xinyue.icu

TS:   s.split(",")
来源：http://zhx.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hxm.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lmh.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://snm.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jok.52xcode.cn

[E08] 数组按分隔符合并
来源：http://nfb.zhongyouzk.top

Py:   ",".join(items)
来源：http://xln.iojbl.cn

PHP:  implode(",", $items);
来源：http://eef.cqqwz.cn

JS:   items.join(",")
来源：http://noz.0kj1m.cn

TS:   items.join(",")
来源：http://rbz.epnwcf.com

Java: String.join(",", items)
来源：http://rna.yongpay.top

Go:   strings.Join(items, ",")
来源：http://ogq.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://uyd.cqqwz.cn

C#:   string.Join(",", items)
来源：http://eoj.yueranfly.top

[E09] 去除所有空白字符
来源：http://kps.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://igg.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://foi.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://vjw.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://xot.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://pwg.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ugb.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gxs.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cku.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://sqo.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dlh.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rzu.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://kzb.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://fqx.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://kly.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bcd.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lcr.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://usv.chenzaomai.com

[E11] 反转字符串
来源：http://adx.yueranfly.top

Py:   s[::-1]
来源：http://jha.smart0.xyz

PHP:  strrev($s);
来源：http://cfl.daxiang520.top


<!-- 参考信息 -->