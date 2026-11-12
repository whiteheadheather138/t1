代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://apd.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://exj.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rxr.aizwys.cn

[D02] 追加元素到末尾
来源：http://nty.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://emp.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yla.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://cny.nanxinkj.top

TS:   arr.push(4);
来源：http://tin.nwbrower.top

Java: list.add(4);
来源：http://wqz.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://fjz.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://cyy.yuxming.cn

C#:   list.Add(4);
来源：http://mtg.cucudq.cn

[D03] 在指定位置插入元素
来源：http://tvi.sweek.top

Py:   arr.insert(0, 0)
来源：http://dto.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fhe.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxj.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://lzs.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://ygu.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://xre.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aoy.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://mko.sjlbkw.cn

[D04] 删除元素
来源：http://ckl.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dpr.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kzj.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wqe.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://ifk.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rxl.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mwo.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kxf.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yfv.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://jmr.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gxm.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dny.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jat.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://vbx.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://tvk.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://eum.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cmi.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uqn.daria6918.cn

[D06] 数组长度
来源：http://smd.zdqjudy.top

Py:   len(arr)
来源：http://uvp.gotoacloud.top

PHP:  count($arr);
来源：http://hfn.yj202588.top

JS:   arr.length
来源：http://vbo.feifeiyinyue.top

TS:   arr.length
来源：http://ono.aizwys.cn

Java: list.size();
来源：http://rfz.yuanzhike.top

Go:   len(arr)
来源：http://bze.xylfe.cn

Ruby: arr.length; arr.size
来源：http://blq.hongshengwenyu.top

C#:   list.Count;
来源：http://clk.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://dyp.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vfw.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://hmo.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://zaj.tarul.cn

TS:   arr.slice(1, 4);
来源：http://ekt.iojbl.cn

Java: list.subList(1, 4);
来源：http://ucn.9152youxi.cn

Go:   arr[1:4]
来源：http://jnn.aibaodan.cn

Ruby: arr[1, 3]
来源：http://btr.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://ujf.ppjwa.cn

[D08] 合并两个数组
来源：http://fyp.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://wck.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://ket.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://coa.jqgfzy.top

TS:   [...a, ...b];
来源：http://nzf.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://huj.xziqi.cn

Go:   append(a, b...)
来源：http://geq.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://upp.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://wzk.yj20258888.top

[D09] 排序（升序）
来源：http://veq.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://gld.fehbvm.com

PHP:  sort($arr);
来源：http://zoy.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ldf.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xja.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jzl.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aax.andypj.xyz

Ruby: arr.sort
来源：http://dzb.epnwcf.com

C#:   list.Sort();
来源：http://bqa.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rsc.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ziq.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://swp.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gws.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rez.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gpc.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yfs.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://njr.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tyy.gotoacloud.top

[D11] 反转数组
来源：http://mgr.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://acs.cheryme.top

PHP:  array_reverse($arr);
来源：http://llr.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zeu.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://ruh.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://dkn.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://uxw.ctjpmb.com

Ruby: arr.reverse
来源：http://qqa.tianlin.xyz

C#:   list.Reverse();
来源：http://odz.hfpthk.cn

[D12] 查找元素下标
来源：http://udc.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://uni.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rxs.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rqs.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ktw.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wvh.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://ihg.jinqigufen.top

Ruby: arr.index(x)
来源：http://qfz.havefunace.top

C#:   list.IndexOf(x);
来源：http://cov.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://vci.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ztf.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lda.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://xpv.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://vpx.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eps.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rvh.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://crw.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rtq.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://qdv.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bfy.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tig.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://lie.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://nzj.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yui.hnqzz.top

Go:   // 手写循环
来源：http://hxo.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://xjo.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ljq.havefunace.top

[D15] 去重
来源：http://lfh.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ogj.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://zgy.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://xue.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://vrv.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://psn.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://isb.jlsjyb.cn

Ruby: arr.uniq
来源：http://psr.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://xiv.gotoacloud.top

[D16] 求和与平均值
来源：http://skx.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://agv.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eji.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lhp.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://una.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xkz.bbcook.cn

Go:   // 手写循环累加
来源：http://esb.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vqv.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://ifw.hysaishi.cn

[D17] 最大值与最小值
来源：http://kim.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://afh.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://tlt.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pjr.zdqjudy.top

TS:   Math.max(...arr);
来源：http://pan.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rrw.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fzj.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://ldj.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://wtt.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://vhg.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jnt.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://xlg.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://npw.vqdsnc.cn

TS:   nested.flat();
来源：http://fcw.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pjg.hnqzz.top

Go:   // 手写双层循环
来源：http://abr.316326.xyz

Ruby: nested.flatten
来源：http://fih.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ily.zhiwuduotai.top

[D19] 按字段分组
来源：http://rpo.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lpz.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nlq.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ooh.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://upl.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ewv.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://hyz.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://heu.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sgm.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://ydm.hammf.cn

Py:   Counter(arr)
来源：http://ifj.cheryme.top

PHP:  array_count_values($arr);
来源：http://xdw.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bdf.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ite.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mrs.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://cry.xinyue.icu

Ruby: arr.tally
来源：http://cvj.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ktf.yj20258888.top

[D21] 判断是否包含某元素
来源：http://cll.yangfankeji.com

Py:   x in arr
来源：http://dbz.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://zpe.fehbvm.com

JS:   arr.includes(x)
来源：http://zzu.uphjek.com

TS:   arr.includes(x)
来源：http://zov.zhijiandao.cn

Java: list.contains(x)
来源：http://jaa.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://vgt.cdnleiting.top

Ruby: arr.include?(x)
来源：http://clf.zdbjq.cn

C#:   list.Contains(x)
来源：http://yeh.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://gys.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mfz.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hdu.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfq.dianchejie.cn

TS:   [...arr];
来源：http://toi.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://qxt.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://zix.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://lsw.cucudq.cn

C#:   new List<int>(list);
来源：http://laj.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://ehq.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vhb.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zyy.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqs.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vgu.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ecf.ybcxt.top

Go:   // 手写循环
来源：http://plo.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qak.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eom.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://pza.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://azj.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pew.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qvo.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rfw.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ahh.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ciq.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ioz.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qqo.hammf.cn

[D25] Set 集合去重与交并差
来源：http://zac.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pgf.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fts.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wry.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://faq.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://erc.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qui.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fgb.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yco.chenjidiqi.icu

[D26] 数组转字符串
来源：http://rzi.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://ljv.yj20258.top

PHP:  implode(", ", $arr);
来源：http://oem.bjfxy.top

JS:   arr.join(", ")
来源：http://udo.guowangkeji.top

TS:   arr.join(", ")
来源：http://jpv.jlsjyb.cn

Java: String.join(", ", list)
来源：http://dug.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://rez.chenzaomai.com

Ruby: arr.join(", ")
来源：http://gza.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://lzu.zhixingplan.top

================================================================================
来源：http://lbj.fengsongda.top

E. 字符串处理
来源：http://xhg.sysykeji.top

================================================================================
来源：http://goc.hnqzz.top

[E01] 拼接字符串
来源：http://cfw.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gzo.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qbp.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dlt.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zem.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hbl.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yve.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mdb.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rru.jiagoushi.top

[E02] 重复字符串
来源：http://bxj.gotoacloud.top

Py:   "ab" * 3
来源：http://ggx.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://qzy.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://xpv.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://ppf.jianghu66.top

Java: "ab".repeat(3)
来源：http://foj.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://hfb.jianghu66.top

Ruby: "ab" * 3
来源：http://wfx.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wdt.fanxiaobao.xyz

[E03] 截取子串
来源：http://num.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blr.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cbr.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gup.xylfe.cn

TS:   s.slice(1, 4)
来源：http://nyt.sweek.top

Java: s.substring(1, 4)
来源：http://gyt.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lim.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://bjm.cashguo.top

C#:   s.Substring(1, 3)
来源：http://iqv.jqgufenzy.top

[E04] 查找子串位置
来源：http://bgp.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://jnp.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://xnm.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://omi.bbcook.cn

TS:   s.indexOf("x")
来源：http://tri.gogol.net.cn

Java: s.indexOf("x")
来源：http://est.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://bfr.nanxuanxn.top

Ruby: s.index("x")
来源：http://xwk.yj20258888.top

C#:   s.IndexOf("x")
来源：http://jai.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wve.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rwr.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lkq.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://caa.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nee.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rqe.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hmc.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xuw.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bzq.zhijiandao.cn

[E06] 替换子串
来源：http://kfl.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yze.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://rxo.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://icy.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://mdc.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vve.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gue.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ntx.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://gyz.dianchejie.cn

[E07] 按分隔符拆分
来源：http://cze.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cdo.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://loa.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zao.shanyushiyangtech.top

TS:   s.split(",")
来源：http://bxf.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jgb.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fgw.yongpay.top

Ruby: s.split(",");  s.split
来源：http://jdl.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tru.smart0.xyz

[E08] 数组按分隔符合并
来源：http://hul.ppjwa.cn

Py:   ",".join(items)
来源：http://exp.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://xpr.meibo888.top

JS:   items.join(",")
来源：http://wjy.xylfe.cn

TS:   items.join(",")
来源：http://pdx.fktsv.cn

Java: String.join(",", items)
来源：http://jhr.bbcook.cn


<!-- 参考信息 -->