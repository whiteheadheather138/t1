代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nsa.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tvk.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://bbu.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jjv.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://iuz.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://oqy.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xlg.chenzaomai.com

[D02] 追加元素到末尾
来源：http://yww.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qht.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ojb.yfazqb.com

JS:   arr.push(4);
来源：http://zku.hcnkem.com

TS:   arr.push(4);
来源：http://hxt.pycfn.com

Java: list.add(4);
来源：http://fqn.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://nse.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://dil.yj20258.top

C#:   list.Add(4);
来源：http://coa.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://hdt.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://tpp.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ydt.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ipz.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://igf.jqgfzy.top

Java: list.add(0, 0);
来源：http://ati.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dtx.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nai.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://woz.xinyue.icu

[D04] 删除元素
来源：http://mso.mhx1999.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fvj.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ihp.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uej.ivvv.top

TS:   arr.splice(0, 1);
来源：http://ahm.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kyp.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qmx.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bsb.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wpc.xinyue.icu

[D05] 访问与修改元素
来源：http://fop.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ybr.ppjwa.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sbf.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zuy.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://afj.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://yqh.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://nux.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tnr.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ygn.svipenyu.cn

[D06] 数组长度
来源：http://jro.hcnkem.com

Py:   len(arr)
来源：http://rva.cashguo.top

PHP:  count($arr);
来源：http://ioo.cashguo.top

JS:   arr.length
来源：http://jmj.sufxvd.cn

TS:   arr.length
来源：http://nze.shanyushiyangkeji.top

Java: list.size();
来源：http://kiy.vqdsnc.cn

Go:   len(arr)
来源：http://rfu.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://zci.snrcjt.cn

C#:   list.Count;
来源：http://beq.c1oappe.top

[D07] 切片 / 取子数组
来源：http://plj.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fhu.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://kip.uphjek.com

JS:   arr.slice(1, 4);
来源：http://okj.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://hgf.fktsv.cn

Java: list.subList(1, 4);
来源：http://cxi.hesvh.cn

Go:   arr[1:4]
来源：http://fub.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://ceg.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://xca.ydjk.org.cn

[D08] 合并两个数组
来源：http://roz.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://kzj.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://zhv.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rfr.sysykeji.top

TS:   [...a, ...b];
来源：http://oka.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lrv.zdqjudy.top

Go:   append(a, b...)
来源：http://msi.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://rft.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://xtp.tianlin.xyz

[D09] 排序（升序）
来源：http://rev.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://ijm.zhongyouzk.top

PHP:  sort($arr);
来源：http://uuf.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gaj.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yqe.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://umj.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rwn.yuanzhike.top

Ruby: arr.sort
来源：http://zic.ivvv.top

C#:   list.Sort();
来源：http://hoe.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://qwb.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://epk.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jhs.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gjx.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zui.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ial.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lnv.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jck.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yht.ydzc1.top

[D11] 反转数组
来源：http://adn.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://vjh.yonumen.top

PHP:  array_reverse($arr);
来源：http://jyg.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sku.sufxvd.cn

TS:   [...arr].reverse();
来源：http://vuk.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://gbr.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://zkf.yj20258.top

Ruby: arr.reverse
来源：http://vxs.cashguo.top

C#:   list.Reverse();
来源：http://oys.jiagoushi.top

[D12] 查找元素下标
来源：http://hwp.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://beg.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cdj.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://esw.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jvc.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ktk.tanke756.top

Go:   slices.Index(arr, x)
来源：http://nif.yj20258888.top

Ruby: arr.index(x)
来源：http://qfv.iojbl.cn

C#:   list.IndexOf(x);
来源：http://aqc.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://qlw.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mog.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rox.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://rhn.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://qdc.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://esu.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mvl.yueranfly.top

Ruby: arr.select { |x| x > 3 }
来源：http://sux.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://loy.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://okh.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ixc.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xyk.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://zdw.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://owt.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mew.bbcook.cn

Go:   // 手写循环
来源：http://vbq.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://exj.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xrv.havefunace.top

[D15] 去重
来源：http://urr.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bfg.bjfxy.top

PHP:  array_unique($arr);
来源：http://mgi.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://jev.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://ivd.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lkz.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://dmy.chenjidiqi.icu

Ruby: arr.uniq
来源：http://xqy.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://kye.andypj.xyz

[D16] 求和与平均值
来源：http://xtf.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysv.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://coa.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hia.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ykf.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://evv.fktsv.cn

Go:   // 手写循环累加
来源：http://iwk.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hih.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://hrq.hesvh.cn

[D17] 最大值与最小值
来源：http://vjb.316326.xyz

Py:   max(arr);  min(arr)
来源：http://ypl.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://pob.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cux.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://hwa.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hiv.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vnc.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://pio.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://ntf.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://vtz.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ygq.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://boo.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mwg.tian-w.cn

TS:   nested.flat();
来源：http://wfw.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://okj.dashuyun.cn

Go:   // 手写双层循环
来源：http://wvv.wangshuangyany.cn

Ruby: nested.flatten
来源：http://lxy.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iqh.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://lir.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gtw.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cdt.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ukz.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jqp.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lss.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://eit.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vet.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bra.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://tms.yj20258888.top

Py:   Counter(arr)
来源：http://szy.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://xqq.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvr.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tkq.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xyq.sweek.top

Go:   // 手写 map[T]int
来源：http://lnx.jinghuilouyu.cn

Ruby: arr.tally
来源：http://fhm.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tge.hnqzz.top

[D21] 判断是否包含某元素
来源：http://pwd.ivvv.top

Py:   x in arr
来源：http://olh.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://aza.vqdsnc.cn

JS:   arr.includes(x)
来源：http://poh.nanxinkj.top

TS:   arr.includes(x)
来源：http://hbs.vqdsnc.cn

Java: list.contains(x)
来源：http://vfk.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://zpi.xinyue.icu

Ruby: arr.include?(x)
来源：http://uhm.jinqigfzy.top

C#:   list.Contains(x)
来源：http://htj.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://xno.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sju.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://src.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://otx.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://qxw.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://mvx.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://buz.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://gkk.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://xzd.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://uys.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pmu.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mgk.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zaw.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bku.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://tpo.smart0.xyz

Go:   // 手写循环
来源：http://mth.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fgl.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://khw.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://prj.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gyc.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://psk.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jaq.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qdq.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ywr.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uec.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pfk.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wvu.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://cjh.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rec.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aka.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kai.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cag.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://alk.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zxu.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qxc.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cwj.yonumen.top

[D26] 数组转字符串
来源：http://wzj.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://aer.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://yiw.jlsjyb.cn

JS:   arr.join(", ")
来源：http://fnl.andypj.xyz

TS:   arr.join(", ")
来源：http://kku.fktsv.cn

Java: String.join(", ", list)
来源：http://ubd.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://dqd.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://ivj.tarul.cn

C#:   string.Join(", ", list)
来源：http://vys.pengpengdd.cyou

================================================================================
来源：http://vam.pengpengdd.cyou

E. 字符串处理
来源：http://tsb.tianlin.xyz

================================================================================
来源：http://wmh.yfazqb.com

[E01] 拼接字符串
来源：http://omz.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mhq.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tcs.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wyr.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://keu.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eam.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pct.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oga.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nhy.jiagoushi.top

[E02] 重复字符串
来源：http://uvf.dashuyun.cn

Py:   "ab" * 3
来源：http://ybn.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://wzp.fehbvm.com

JS:   "ab".repeat(3)
来源：http://bwv.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://qkb.jiagoushi.top

Java: "ab".repeat(3)
来源：http://uwh.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://cxz.xinyue.icu

Ruby: "ab" * 3
来源：http://tmu.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wux.yonumen.top

[E03] 截取子串
来源：http://ezz.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ppj.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nvm.pycfn.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://niv.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://zdz.zdbjq.cn

Java: s.substring(1, 4)
来源：http://tkh.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uqs.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://ijk.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://hir.daxiang520.top

[E04] 查找子串位置
来源：http://ebl.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://ueu.yongpay.top

PHP:  strpos($s, "x");
来源：http://xzq.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fpz.tarul.cn

TS:   s.indexOf("x")
来源：http://kix.pycfn.com

Java: s.indexOf("x")
来源：http://ies.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://ixm.guowangkeji.top

Ruby: s.index("x")
来源：http://xgk.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://kua.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cxp.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://puy.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vgx.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uft.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://hvu.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qfl.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zqm.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://swt.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pdi.zhijiandao.cn

[E06] 替换子串
来源：http://flx.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pto.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://qab.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gxd.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://lfj.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tcd.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sod.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fvq.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://cul.hnqzz.top

[E07] 按分隔符拆分
来源：http://vkn.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hmw.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tpw.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://znu.dianchejie.cn

TS:   s.split(",")
来源：http://djf.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qzj.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wop.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://cdp.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gsz.daxiang520.top

[E08] 数组按分隔符合并
来源：http://dzf.xziqi.cn

Py:   ",".join(items)
来源：http://ecv.hesvh.cn


<!-- 参考信息 -->