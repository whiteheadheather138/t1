代发 wailian999

C#:   list.Insert(0, 0);
来源：http://gqm.meibo888.top

[D04] 删除元素
来源：http://act.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rpf.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wpp.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vqb.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://hdz.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hsw.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lfx.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iou.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ohi.zdbjq.cn

[D05] 访问与修改元素
来源：http://uyo.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xbj.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pny.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hut.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://avh.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://nej.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ect.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://agp.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iti.yvedp.cn

[D06] 数组长度
来源：http://gaa.0kj1m.cn

Py:   len(arr)
来源：http://rgb.316326.xyz

PHP:  count($arr);
来源：http://nxq.shangyingyoupin.top

JS:   arr.length
来源：http://ati.jianghu66.top

TS:   arr.length
来源：http://eut.bjfxy.top

Java: list.size();
来源：http://sqv.fktsv.cn

Go:   len(arr)
来源：http://nkc.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://ebr.yvedp.cn

C#:   list.Count;
来源：http://awx.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://llo.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yfr.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rml.ivvv.top

JS:   arr.slice(1, 4);
来源：http://rax.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://ywt.xinyue.icu

Java: list.subList(1, 4);
来源：http://hfw.52xcode.cn

Go:   arr[1:4]
来源：http://ffa.pycfn.com

Ruby: arr[1, 3]
来源：http://uhe.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://mko.meibo888.top

[D08] 合并两个数组
来源：http://mit.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://qpp.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://gmo.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://eae.smart0.xyz

TS:   [...a, ...b];
来源：http://hmn.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://llp.nanxuanxn.top

Go:   append(a, b...)
来源：http://efe.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://sdt.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://mpw.zhongyouzk.top

[D09] 排序（升序）
来源：http://gpo.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://zef.vehdjk.com

PHP:  sort($arr);
来源：http://uul.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dvf.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ked.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bjg.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gid.gogol.net.cn

Ruby: arr.sort
来源：http://ost.yonumen.top

C#:   list.Sort();
来源：http://cma.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://hdw.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zbh.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pzt.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://irj.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vxf.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hgl.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bvq.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aqs.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vbn.yvedp.cn

[D11] 反转数组
来源：http://ejk.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://lyy.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://usn.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zlx.smart0.xyz

TS:   [...arr].reverse();
来源：http://imk.hnqzz.top

Java: Collections.reverse(list);
来源：http://rzv.sweek.top

Go:   slices.Reverse(arr)
来源：http://anq.hcnkem.com

Ruby: arr.reverse
来源：http://hhi.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://faq.shuidangran.top

[D12] 查找元素下标
来源：http://zcg.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://bbn.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zwa.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uzj.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdg.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tdz.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://dln.nanxuanxn.top

Ruby: arr.index(x)
来源：http://pon.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://tmi.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://ogb.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ycd.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lsi.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://mwt.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://zln.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zdb.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aes.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sug.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ybk.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://dvn.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ras.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qyf.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://ahd.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://ozv.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://kfw.fanxiaobao.xyz

Go:   // 手写循环
来源：http://hrk.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://yxr.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eql.yueranfly.top

[D15] 去重
来源：http://sbg.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xde.jiagoushi.top

PHP:  array_unique($arr);
来源：http://alo.ydzc1.top

JS:   [...new Set(arr)]
来源：http://ycp.yvedp.cn

TS:   [...new Set(arr)]
来源：http://vxi.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bmh.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://mbu.zdqjudy.top

Ruby: arr.uniq
来源：http://ayq.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://kmq.sufxvd.cn

[D16] 求和与平均值
来源：http://ldt.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xsk.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uft.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iii.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tqb.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cpz.9152youxi.cn

Go:   // 手写循环累加
来源：http://nkx.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vme.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://fzp.fengsongda.top

[D17] 最大值与最小值
来源：http://rtb.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://wqi.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://zsq.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zdn.wangdashe.top

TS:   Math.max(...arr);
来源：http://gzt.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hik.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxs.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://cha.sweek.top

C#:   list.Max();  list.Min()
来源：http://hou.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://yqi.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ize.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://itt.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xcp.yfazqb.com

TS:   nested.flat();
来源：http://adf.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pds.ivvv.top

Go:   // 手写双层循环
来源：http://mnk.epnwcf.com

Ruby: nested.flatten
来源：http://vfm.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wwq.zhiwuduotai.top

[D19] 按字段分组
来源：http://dlf.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mxk.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://snn.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wtp.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mug.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tkw.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://tuj.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mhc.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ejo.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://vsi.shuidangran.top

Py:   Counter(arr)
来源：http://ssv.cucudq.cn

PHP:  array_count_values($arr);
来源：http://ejq.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://stl.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uhu.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://orw.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://lzg.fengsongda.top

Ruby: arr.tally
来源：http://edi.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dbq.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://jsb.chenzaomai.com

Py:   x in arr
来源：http://khm.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://tvs.fzhhl.top

JS:   arr.includes(x)
来源：http://cdb.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://xvh.ydjk.org.cn

Java: list.contains(x)
来源：http://gcw.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://jsa.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://qkj.daria6918.cn

C#:   list.Contains(x)
来源：http://enk.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://ipn.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gom.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tyz.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wvd.xuanzx.com

TS:   [...arr];
来源：http://lwx.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://rje.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://enq.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://tez.hnxiangtu.top

C#:   new List<int>(list);
来源：http://lgs.jianghu66.top

[D23] reduce 累积计算
来源：http://sfk.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyf.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lxt.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ubd.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xty.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qll.guannengcc.top

Go:   // 手写循环
来源：http://cfr.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sfs.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xlc.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://cqe.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kkd.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jad.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://azz.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yot.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qnq.aibaodan.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://syb.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tnx.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vdq.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://xms.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hfr.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dgj.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://suo.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gdz.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fpk.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vdr.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqe.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dbk.daria6918.cn

[D26] 数组转字符串
来源：http://obg.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://ugq.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://jya.yuxming.cn

JS:   arr.join(", ")
来源：http://ejj.haohaochexian.top

TS:   arr.join(", ")
来源：http://tru.pycfn.com

Java: String.join(", ", list)
来源：http://gyp.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://erg.svipenyu.cn

Ruby: arr.join(", ")
来源：http://qpe.yfazqb.com

C#:   string.Join(", ", list)
来源：http://wuk.tian-w.cn

================================================================================
来源：http://djg.fehbvm.com

E. 字符串处理
来源：http://ouc.jiagoushi.top

================================================================================
来源：http://zpw.gzhubu.top

[E01] 拼接字符串
来源：http://kez.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rzr.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://amd.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vmn.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nht.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rbb.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ybj.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tkb.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hvf.yj20258888.top

[E02] 重复字符串
来源：http://dwd.aizwys.cn

Py:   "ab" * 3
来源：http://dby.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://zhs.andypj.xyz

JS:   "ab".repeat(3)
来源：http://rdl.xinyue.icu

TS:   "ab".repeat(3)
来源：http://cdo.0kj1m.cn

Java: "ab".repeat(3)
来源：http://nmi.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://hcx.svipenyu.cn

Ruby: "ab" * 3
来源：http://vzb.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nds.zhixingplan.top

[E03] 截取子串
来源：http://zwy.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://avo.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jof.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zih.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://fwo.havefunace.top

Java: s.substring(1, 4)
来源：http://cxq.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nri.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gom.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://bhf.hongshengwenyu.top

[E04] 查找子串位置
来源：http://mag.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://ugf.fzhhl.top

PHP:  strpos($s, "x");
来源：http://dxf.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fec.sufxvd.cn

TS:   s.indexOf("x")
来源：http://ixu.haohaochexian.top

Java: s.indexOf("x")
来源：http://meb.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://pss.zycfv.cn

Ruby: s.index("x")
来源：http://wye.ybcxt.top

C#:   s.IndexOf("x")
来源：http://shu.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nei.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xhi.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kvd.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fiw.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://pas.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pyg.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://opg.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aap.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sgk.shanyushiyangkeji.top

[E06] 替换子串
来源：http://aos.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mox.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://oiq.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbd.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://rlo.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cih.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jxu.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://icp.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://ttm.yueranfly.top

[E07] 按分隔符拆分
来源：http://are.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nev.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lkg.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cxj.sweek.top

TS:   s.split(",")
来源：http://zae.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://abd.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sbo.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://grw.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xzd.ivvv.top

[E08] 数组按分隔符合并
来源：http://tiy.zhixingplan.top

Py:   ",".join(items)
来源：http://gix.mhx1999.top

PHP:  implode(",", $items);
来源：http://mjf.yanxiufei.cn

JS:   items.join(",")
来源：http://enn.sxryk.cn

TS:   items.join(",")
来源：http://irt.cqqwz.cn

Java: String.join(",", items)
来源：http://jcb.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://vex.shangyingyoupin.top

Ruby: items.join(",")
来源：http://quq.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://tjx.mhx1999.top

[E09] 去除所有空白字符
来源：http://kcx.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eck.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://idf.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://vil.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://xrc.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://ueo.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rad.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://yqp.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ysc.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://usq.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wcz.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xar.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://bnf.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://fkd.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://qia.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jed.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://euk.gogol.net.cn


<!-- 参考信息 -->