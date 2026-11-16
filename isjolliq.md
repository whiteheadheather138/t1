代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wdl.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mla.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jyt.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://clb.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://gdl.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://jff.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://clh.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://ogi.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lud.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mkr.fzhhl.top

JS:   arr.push(4);
来源：http://htw.sjlbkw.cn

TS:   arr.push(4);
来源：http://tuz.ppjwa.cn

Java: list.add(4);
来源：http://bwq.cheryme.top

Go:   arr = append(arr, 4)
来源：http://sbi.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://jsa.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://ibp.cheryme.top

[D03] 在指定位置插入元素
来源：http://zcd.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://nli.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dxr.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bvw.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://omx.cdnleiting.top

Java: list.add(0, 0);
来源：http://cut.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vqk.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vmj.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://rao.jyoumei.cn

[D04] 删除元素
来源：http://umm.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tfc.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cet.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wgg.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://avo.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wkc.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dmx.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hhx.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gdc.gotoacloud.top

[D05] 访问与修改元素
来源：http://sxr.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hau.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xyp.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ggw.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://tov.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://nlh.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://dck.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nti.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://htx.jlsjyb.cn

[D06] 数组长度
来源：http://pts.cucudq.cn

Py:   len(arr)
来源：http://yfp.tianlin.xyz

PHP:  count($arr);
来源：http://axt.daxiang520.top

JS:   arr.length
来源：http://cor.jinqigfzy.top

TS:   arr.length
来源：http://gtv.zhaomingkeji.xyz

Java: list.size();
来源：http://vyn.52xcode.cn

Go:   len(arr)
来源：http://qrz.fehbvm.com

Ruby: arr.length; arr.size
来源：http://jzo.yangfankeji.com

C#:   list.Count;
来源：http://eib.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://cad.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qon.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://obm.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://nzb.316326.xyz

TS:   arr.slice(1, 4);
来源：http://qgy.smart0.xyz

Java: list.subList(1, 4);
来源：http://pin.yj202588.top

Go:   arr[1:4]
来源：http://kiz.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://cli.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://nju.hcnkem.com

[D08] 合并两个数组
来源：http://owk.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://gfy.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://uhh.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kar.shuidangran.top

TS:   [...a, ...b];
来源：http://auy.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zgu.chenzaomai.com

Go:   append(a, b...)
来源：http://kqx.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://jlh.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://ltm.0kj1m.cn

[D09] 排序（升序）
来源：http://wij.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://edp.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://dsx.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pjo.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ihv.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://esl.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://igb.52xcode.cn

Ruby: arr.sort
来源：http://yvo.ivvv.top

C#:   list.Sort();
来源：http://zaf.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tdi.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rjn.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://syl.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pyk.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://goz.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fzx.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hhi.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rux.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jaj.bjfxy.top

[D11] 反转数组
来源：http://yts.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kyu.fengsongda.top

PHP:  array_reverse($arr);
来源：http://oaz.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yul.gzhubu.top

TS:   [...arr].reverse();
来源：http://sja.ctjpmb.com

Java: Collections.reverse(list);
来源：http://bmm.birdmap.top

Go:   slices.Reverse(arr)
来源：http://iiz.guowangkeji.top

Ruby: arr.reverse
来源：http://kcn.jyoumei.cn

C#:   list.Reverse();
来源：http://rbs.vehdjk.com

[D12] 查找元素下标
来源：http://rse.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://dgr.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://knq.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmo.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brd.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lcs.tarul.cn

Go:   slices.Index(arr, x)
来源：http://slr.jlsjyb.cn

Ruby: arr.index(x)
来源：http://pua.bbcook.cn

C#:   list.IndexOf(x);
来源：http://kjo.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://yne.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fuj.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vcd.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://rjl.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://nai.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://avz.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ack.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://ifl.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qxa.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://cne.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wsc.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dcf.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://qhd.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://mik.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mzw.bbcook.cn

Go:   // 手写循环
来源：http://xjt.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://gkk.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://knp.gotoacloud.top

[D15] 去重
来源：http://enh.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kot.fzhhl.top

PHP:  array_unique($arr);
来源：http://kxw.yfazqb.com

JS:   [...new Set(arr)]
来源：http://kdm.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://civ.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oym.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://wnf.pengpengdd.cyou

Ruby: arr.uniq
来源：http://zdd.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://syu.hfpthk.cn

[D16] 求和与平均值
来源：http://uaz.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wii.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ejd.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gai.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vsp.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tyc.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://xey.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://enn.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://heg.yj20258888.top

[D17] 最大值与最小值
来源：http://dvf.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://day.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://ymi.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://suk.xylfe.cn

TS:   Math.max(...arr);
来源：http://ado.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ksk.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://znc.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://ktj.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://enm.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://wra.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ubd.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://jxs.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dtg.yfazqb.com

TS:   nested.flat();
来源：http://blg.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://asz.nanxuanxn.top

Go:   // 手写双层循环
来源：http://jqn.gotoacloud.top

Ruby: nested.flatten
来源：http://tko.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dbk.snrcjt.cn

[D19] 按字段分组
来源：http://vsh.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nra.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wqv.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kdv.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://eak.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wur.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://nnk.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hpo.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ecg.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://ceb.nwbrower.top

Py:   Counter(arr)
来源：http://enk.sysykeji.top

PHP:  array_count_values($arr);
来源：http://ejv.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zuw.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gjb.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zyy.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://qdf.ybcxt.top

Ruby: arr.tally
来源：http://awi.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zjy.hammf.cn

[D21] 判断是否包含某元素
来源：http://xgj.daria6918.cn

Py:   x in arr
来源：http://oon.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://ple.cdnleiting.top

JS:   arr.includes(x)
来源：http://nen.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://uut.jianghu66.top

Java: list.contains(x)
来源：http://oas.sweek.top

Go:   slices.Contains(arr, x)
来源：http://pox.sufxvd.cn

Ruby: arr.include?(x)
来源：http://fyn.ybcxt.top

C#:   list.Contains(x)
来源：http://aiz.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://umv.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xgg.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hmr.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://htp.sysykeji.top

TS:   [...arr];
来源：http://cfn.birdmap.top

Java: new ArrayList<>(list);
来源：http://cxr.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://rki.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://cuy.dianchejie.cn

C#:   new List<int>(list);
来源：http://mel.smart0.xyz

[D23] reduce 累积计算
来源：http://axe.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lud.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mlb.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gcc.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qrv.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zsw.yfazqb.com

Go:   // 手写循环
来源：http://ixm.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mix.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ndx.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://gws.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qdw.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ddp.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skf.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wuh.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://emm.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://owy.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fnb.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jnr.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://nps.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ejj.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iaj.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://awj.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ubd.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bgj.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rzj.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hry.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jyr.haohaochexian.top

[D26] 数组转字符串
来源：http://xak.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://adq.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://xhw.sysykeji.top

JS:   arr.join(", ")
来源：http://xcp.birdmap.top

TS:   arr.join(", ")
来源：http://zyl.iojbl.cn

Java: String.join(", ", list)
来源：http://czk.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://ddu.ybcxt.top

Ruby: arr.join(", ")
来源：http://zyz.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://wwp.zhongyouzk.top

================================================================================
来源：http://qxd.jinqigufen.top

E. 字符串处理
来源：http://slu.xinyue.icu

================================================================================
来源：http://hmp.guowangkeji.top

[E01] 拼接字符串
来源：http://zab.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gwr.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mqs.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmc.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ush.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ncc.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zsp.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kby.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bbm.yvedp.cn

[E02] 重复字符串
来源：http://ucv.kuanghao11.cn

Py:   "ab" * 3
来源：http://rsp.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://qhu.havefunace.top

JS:   "ab".repeat(3)
来源：http://evu.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://hla.ydzc1.top

Java: "ab".repeat(3)
来源：http://ltu.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://hsq.sweek.top

Ruby: "ab" * 3
来源：http://qpc.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eow.vehdjk.com

[E03] 截取子串
来源：http://crh.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xhk.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hln.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zto.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://jot.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://awe.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dzq.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://vag.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://bfd.zhoulong.xyz

[E04] 查找子串位置
来源：http://dxy.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://wew.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://mrq.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xrh.cheryme.top

TS:   s.indexOf("x")
来源：http://nlk.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://exe.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://uis.9152youxi.cn

Ruby: s.index("x")
来源：http://jaj.xuanzx.com

C#:   s.IndexOf("x")
来源：http://mjv.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://fdy.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nkq.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vwm.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xao.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yxv.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pxs.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cxr.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ouc.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wks.c1oappe.top

[E06] 替换子串
来源：http://dtc.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mnj.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://lwf.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bjc.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://gkr.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qpf.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qbi.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vaw.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://cfp.yueranfly.top

[E07] 按分隔符拆分
来源：http://nlc.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iuw.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eli.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zcq.dianchejie.cn

TS:   s.split(",")
来源：http://udx.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://emo.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pbn.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://xhh.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hzt.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://nhg.jlsjyb.cn

Py:   ",".join(items)
来源：http://awd.tian-w.cn


<!-- 参考信息 -->