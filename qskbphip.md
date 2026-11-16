代发 wailian999

[D03] 在指定位置插入元素
来源：http://xgu.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://ahn.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vax.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fnf.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://pou.ppjwa.cn

Java: list.add(0, 0);
来源：http://laq.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://mhq.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kaq.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://yzk.hywenlv.cn

[D04] 删除元素
来源：http://vop.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pcs.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hlm.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wly.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://xsx.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gja.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pqt.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kzw.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wog.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://cxm.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://umi.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hvg.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xcn.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://vqt.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wtv.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://hwb.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ivw.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oor.sufxvd.cn

[D06] 数组长度
来源：http://tvv.hcnkem.com

Py:   len(arr)
来源：http://sea.aizwys.cn

PHP:  count($arr);
来源：http://qrl.zhaomingkeji.xyz

JS:   arr.length
来源：http://lly.zhoulong.xyz

TS:   arr.length
来源：http://fih.ydjk.org.cn

Java: list.size();
来源：http://abx.jyoumei.cn

Go:   len(arr)
来源：http://lyn.bjfxy.top

Ruby: arr.length; arr.size
来源：http://kzc.jinqigfzy.top

C#:   list.Count;
来源：http://raj.52xcode.cn

[D07] 切片 / 取子数组
来源：http://aeo.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyd.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://ite.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://nfs.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://ltp.meibo888.top

Java: list.subList(1, 4);
来源：http://beh.hywenlv.cn

Go:   arr[1:4]
来源：http://hpo.xziqi.cn

Ruby: arr[1, 3]
来源：http://psq.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://ubb.yj20258888.top

[D08] 合并两个数组
来源：http://kgj.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://cjw.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://jbm.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dbi.gzhubu.top

TS:   [...a, ...b];
来源：http://vzn.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jlx.ctjpmb.com

Go:   append(a, b...)
来源：http://xdm.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://dkq.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://eoy.hnxiangtu.top

[D09] 排序（升序）
来源：http://wjk.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://kdn.daxiang520.top

PHP:  sort($arr);
来源：http://vom.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oio.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bcd.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xrs.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dgc.chenzaomai.com

Ruby: arr.sort
来源：http://mgu.vqdsnc.cn

C#:   list.Sort();
来源：http://srs.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fmw.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wbb.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ifd.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://akh.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpn.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jmg.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://skl.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sgm.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xwj.jinqigfzy.top

[D11] 反转数组
来源：http://wpy.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://mxm.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://ywp.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://udh.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://fsr.pycfn.com

Java: Collections.reverse(list);
来源：http://hfc.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://atl.hcnkem.com

Ruby: arr.reverse
来源：http://zyr.zdbjq.cn

C#:   list.Reverse();
来源：http://oox.xuetiantiany.cn

[D12] 查找元素下标
来源：http://xku.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://khr.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mji.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://urh.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmz.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zve.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://jgv.daria6918.cn

Ruby: arr.index(x)
来源：http://qgc.cashguo.top

C#:   list.IndexOf(x);
来源：http://sje.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://osa.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://den.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sie.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://erp.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://qxr.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tcf.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://klc.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://zyj.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aat.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://jaq.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iar.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://irv.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://nsp.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://chw.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ywe.ydzc1.top

Go:   // 手写循环
来源：http://ktt.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://iae.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sdk.pengpengdd.cyou

[D15] 去重
来源：http://uci.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pgf.9152youxi.cn

PHP:  array_unique($arr);
来源：http://tlj.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://jfx.sxryk.cn

TS:   [...new Set(arr)]
来源：http://dzp.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gjs.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://itm.cdnleiting.top

Ruby: arr.uniq
来源：http://hnm.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://zbo.epnwcf.com

[D16] 求和与平均值
来源：http://kmy.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xbs.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://whj.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydo.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wav.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fyo.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://jbx.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bgi.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://icf.vehdjk.com

[D17] 最大值与最小值
来源：http://blc.hammf.cn

Py:   max(arr);  min(arr)
来源：http://vxj.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://fnk.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jmf.bjfxy.top

TS:   Math.max(...arr);
来源：http://uxd.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nbk.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ccp.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://ikm.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://tnx.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://wac.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dki.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://tni.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nuq.zhongyouzk.top

TS:   nested.flat();
来源：http://oat.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sts.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://yxl.meibo888.top

Ruby: nested.flatten
来源：http://fej.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xks.haohaochexian.top

[D19] 按字段分组
来源：http://uwe.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eao.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cvo.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://etk.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uun.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mso.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://fph.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sfi.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://inv.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://hfy.jianghu66.top

Py:   Counter(arr)
来源：http://ogr.fzhhl.top

PHP:  array_count_values($arr);
来源：http://xdw.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayr.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pcc.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ghe.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://tpo.chenzaomai.com

Ruby: arr.tally
来源：http://boo.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gjy.aizwys.cn

[D21] 判断是否包含某元素
来源：http://iby.ivvv.top

Py:   x in arr
来源：http://ooz.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://znt.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://epg.vqdsnc.cn

TS:   arr.includes(x)
来源：http://lzr.yfazqb.com

Java: list.contains(x)
来源：http://qnb.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://ycz.sxryk.cn

Ruby: arr.include?(x)
来源：http://xbb.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://dca.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://uwy.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pte.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dhg.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rpk.0kj1m.cn

TS:   [...arr];
来源：http://znn.sweek.top

Java: new ArrayList<>(list);
来源：http://kdr.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://duf.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://gkx.zhengqikj.top

C#:   new List<int>(list);
来源：http://mem.bjfxy.top

[D23] reduce 累积计算
来源：http://pwn.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://odc.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kqf.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vof.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hdx.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ati.meibo888.top

Go:   // 手写循环
来源：http://udq.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wsi.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vjf.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://mvq.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqd.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ykz.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aie.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bzn.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qwz.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://znv.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oqm.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bgg.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://dob.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://scg.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nkw.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kgi.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://taw.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eju.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tsp.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cme.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bzq.9152youxi.cn

[D26] 数组转字符串
来源：http://xff.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://fpk.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://tqn.dianchejie.cn

JS:   arr.join(", ")
来源：http://sqe.vqdsnc.cn

TS:   arr.join(", ")
来源：http://rit.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://nqz.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://tpa.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://jtg.xuanzx.com

C#:   string.Join(", ", list)
来源：http://lww.uphjek.com

================================================================================
来源：http://jch.hesvh.cn

E. 字符串处理
来源：http://ita.sjlbkw.cn

================================================================================
来源：http://qmv.aibaodan.cn

[E01] 拼接字符串
来源：http://chf.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mzk.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mew.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgm.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://skf.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fky.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rhw.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dug.zhiwuduotai.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dap.meibo888.top

[E02] 重复字符串
来源：http://wat.vqdsnc.cn

Py:   "ab" * 3
来源：http://uqd.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://xkz.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://yxf.redwolf501.top

TS:   "ab".repeat(3)
来源：http://zet.yangfankeji.com

Java: "ab".repeat(3)
来源：http://dab.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://kba.xziqi.cn

Ruby: "ab" * 3
来源：http://djd.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hmh.yj20258888.top

[E03] 截取子串
来源：http://qrf.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgn.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cal.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fgk.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://qsx.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://bgl.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sjg.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://oho.sweek.top

C#:   s.Substring(1, 3)
来源：http://xhp.hammf.cn

[E04] 查找子串位置
来源：http://yzz.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://kgl.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://tyh.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qyu.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://tln.yongpay.top

Java: s.indexOf("x")
来源：http://mhh.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://uqc.xziqi.cn

Ruby: s.index("x")
来源：http://mmv.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://ims.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kme.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://agm.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qsh.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cpy.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://xww.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ggm.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ooo.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bmf.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oyv.sxryk.cn

[E06] 替换子串
来源：http://vzs.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dtr.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://xym.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://klf.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://pyb.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxo.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zht.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rhr.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://kdq.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://uyz.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xrd.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aas.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oga.daria6918.cn

TS:   s.split(",")
来源：http://iqw.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://lwa.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zvi.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://sui.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cbb.xinyue.icu

[E08] 数组按分隔符合并
来源：http://nbm.yuxming.cn

Py:   ",".join(items)
来源：http://und.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://dwt.vqdsnc.cn

JS:   items.join(",")
来源：http://xqo.zhongyouzk.top

TS:   items.join(",")
来源：http://ave.tianlin.xyz

Java: String.join(",", items)
来源：http://xku.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://toz.bjfxy.top

Ruby: items.join(",")
来源：http://omc.316326.xyz

C#:   string.Join(",", items)
来源：http://ygs.fzhhl.top

[E09] 去除所有空白字符
来源：http://gza.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mwg.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fxx.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://tye.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://edz.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://ivp.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kmb.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://uwa.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blf.smart0.xyz


<!-- 参考信息 -->