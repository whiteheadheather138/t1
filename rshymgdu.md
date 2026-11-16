代发 wailian999

D. 数组 / 列表 / 集合
来源：http://ypz.pycfn.com

================================================================================
来源：http://gxq.gzhubu.top

[D01] 创建数组 / 列表
来源：http://lul.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yqj.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jpq.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tis.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bev.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mgw.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://qqr.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://mok.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ntf.hcnkem.com

[D02] 追加元素到末尾
来源：http://nrw.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vdf.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zyf.ydzc1.top

JS:   arr.push(4);
来源：http://zqs.uphjek.com

TS:   arr.push(4);
来源：http://iae.hfpthk.cn

Java: list.add(4);
来源：http://cub.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://jwu.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://dsq.fzhhl.top

C#:   list.Add(4);
来源：http://dwo.yvedp.cn

[D03] 在指定位置插入元素
来源：http://jxg.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://lww.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iek.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://opn.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://rpb.haohaochexian.top

Java: list.add(0, 0);
来源：http://qja.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://irp.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dnp.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://mub.fktsv.cn

[D04] 删除元素
来源：http://ydh.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nul.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fqb.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bng.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://qst.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bsf.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ytq.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qtx.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hvi.nanxinkj.top

[D05] 访问与修改元素
来源：http://jmu.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hox.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eqz.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://idn.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://hvw.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://ajj.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://mfj.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ljs.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://was.fanxiaobao.xyz

[D06] 数组长度
来源：http://vbt.daxiang520.top

Py:   len(arr)
来源：http://xjk.yangfankeji.com

PHP:  count($arr);
来源：http://cac.nanxinkj.top

JS:   arr.length
来源：http://boj.yj20258888.top

TS:   arr.length
来源：http://emr.yj20258.top

Java: list.size();
来源：http://mrt.redwolf501.top

Go:   len(arr)
来源：http://rgf.epnwcf.com

Ruby: arr.length; arr.size
来源：http://zaf.hysaishi.cn

C#:   list.Count;
来源：http://ecj.tian-w.cn

[D07] 切片 / 取子数组
来源：http://vjg.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nnk.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://aup.uphjek.com

JS:   arr.slice(1, 4);
来源：http://ylr.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://ooc.ppjwa.cn

Java: list.subList(1, 4);
来源：http://tft.yfazqb.com

Go:   arr[1:4]
来源：http://pdv.iojbl.cn

Ruby: arr[1, 3]
来源：http://lim.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://zha.tian-w.cn

[D08] 合并两个数组
来源：http://tku.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://ggp.tanke756.top

PHP:  array_merge($a, $b);
来源：http://hya.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cok.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://tju.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wpc.sysykeji.top

Go:   append(a, b...)
来源：http://yvp.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://hiq.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://kcm.zhongyouzk.top

[D09] 排序（升序）
来源：http://ejp.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://ues.hfpthk.cn

PHP:  sort($arr);
来源：http://ufv.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sgy.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ptj.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://pja.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xvv.jiagoushi.top

Ruby: arr.sort
来源：http://vru.guannengcc.top

C#:   list.Sort();
来源：http://zxj.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rgw.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rrl.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffk.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zrf.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ryq.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hkj.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fxi.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mvm.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dwj.jinyuanbaomall.cn

[D11] 反转数组
来源：http://ego.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://twy.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://oys.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mpt.ydzc1.top

TS:   [...arr].reverse();
来源：http://jpx.jqgfzy.top

Java: Collections.reverse(list);
来源：http://qpi.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://nch.jinqigufen.top

Ruby: arr.reverse
来源：http://dvg.zhengqikj.top

C#:   list.Reverse();
来源：http://fxp.kuanghao11.cn

[D12] 查找元素下标
来源：http://dap.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://ukj.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ebb.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ewl.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qqb.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://smu.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://tny.redwolf501.top

Ruby: arr.index(x)
来源：http://dud.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://xrz.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://igj.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ogi.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lqd.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://gky.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://uwh.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kgn.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gvp.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://ass.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qio.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://czo.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://foz.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nxj.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://btw.sweek.top

TS:   arr.map(x => x * 2)
来源：http://axd.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fhu.andypj.xyz

Go:   // 手写循环
来源：http://xus.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://fon.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aib.jiagoushi.top

[D15] 去重
来源：http://ntw.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yon.cashguo.top

PHP:  array_unique($arr);
来源：http://llx.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://ouo.aizwys.cn

TS:   [...new Set(arr)]
来源：http://pao.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ydd.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://krg.gotoacloud.top

Ruby: arr.uniq
来源：http://qwh.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://xis.uphjek.com

[D16] 求和与平均值
来源：http://ofn.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyo.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xtw.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpz.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sff.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ncf.yongpay.top

Go:   // 手写循环累加
来源：http://hoy.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oqb.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://tgi.gotoacloud.top

[D17] 最大值与最小值
来源：http://wsc.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://tft.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://hnz.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bsy.aibaodan.cn

TS:   Math.max(...arr);
来源：http://fru.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tlf.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dyb.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://gec.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://tyz.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://eiw.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uwy.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://yry.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kpo.zhijiandao.cn

TS:   nested.flat();
来源：http://wvo.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qrc.hcnkem.com

Go:   // 手写双层循环
来源：http://vkn.chenzaomai.com

Ruby: nested.flatten
来源：http://yud.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yzh.ppjwa.cn

[D19] 按字段分组
来源：http://rgv.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dhm.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rfm.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://avx.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xaa.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ldm.meibo888.top

Go:   // 手写 map[string][]T
来源：http://yyu.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gnn.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hzq.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://wef.hnxiangtu.top

Py:   Counter(arr)
来源：http://rik.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://uks.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgf.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uhb.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cuh.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://wfi.hysaishi.cn

Ruby: arr.tally
来源：http://gjd.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dha.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://qjm.hesvh.cn

Py:   x in arr
来源：http://vdf.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://pbh.xylfe.cn

JS:   arr.includes(x)
来源：http://uwb.9152youxi.cn

TS:   arr.includes(x)
来源：http://ksw.xinyue.icu

Java: list.contains(x)
来源：http://xit.chenlongwang.top

Go:   slices.Contains(arr, x)
来源：http://lpt.fengsongda.top

Ruby: arr.include?(x)
来源：http://ods.uphjek.com

C#:   list.Contains(x)
来源：http://mfj.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://voi.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zve.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kuf.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://syp.jinqigufen.top

TS:   [...arr];
来源：http://zna.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://xag.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yir.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://qmg.xinyue.icu

C#:   new List<int>(list);
来源：http://nlo.yueranfly.top

[D23] reduce 累积计算
来源：http://dui.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vff.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fai.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uom.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vxc.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qbv.0kj1m.cn

Go:   // 手写循环
来源：http://ioj.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sge.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://use.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://xgg.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cjd.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://erd.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vyi.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://joq.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ils.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bej.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ivt.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://meo.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://khg.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whm.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tiz.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tmt.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sva.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qlh.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lyf.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dpm.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uqh.sweek.top

[D26] 数组转字符串
来源：http://eyz.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://xdq.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://alr.jqgufenzy.top

JS:   arr.join(", ")
来源：http://pgg.gzhubu.top

TS:   arr.join(", ")
来源：http://gcw.xuanzx.com

Java: String.join(", ", list)
来源：http://dlq.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://gin.ppjwa.cn

Ruby: arr.join(", ")
来源：http://jpe.andypj.xyz

C#:   string.Join(", ", list)
来源：http://udg.daria6918.cn

================================================================================
来源：http://zct.quarkkingdee.top

E. 字符串处理
来源：http://iue.yueranfly.top

================================================================================
来源：http://ecy.birdmap.top

[E01] 拼接字符串
来源：http://eku.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ips.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dbi.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wje.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ova.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xyy.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://soy.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vrl.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nxl.chenjidiqi.icu

[E02] 重复字符串
来源：http://gjb.pycfn.com

Py:   "ab" * 3
来源：http://cqw.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://qce.tian-w.cn

JS:   "ab".repeat(3)
来源：http://gef.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://svc.svipenyu.cn

Java: "ab".repeat(3)
来源：http://nte.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://rvw.birdmap.top

Ruby: "ab" * 3
来源：http://pqm.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vyp.jinqigufen.top

[E03] 截取子串
来源：http://tcj.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rnf.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oat.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zjl.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://ikm.tanke756.top

Java: s.substring(1, 4)
来源：http://eyi.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wyb.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://wzc.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://hyf.gotoacloud.top

[E04] 查找子串位置
来源：http://jou.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://fhn.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://hss.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rvu.daxiang520.top

TS:   s.indexOf("x")
来源：http://eoi.aizwys.cn

Java: s.indexOf("x")
来源：http://lfr.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://wlv.shzxlz.cn

Ruby: s.index("x")
来源：http://iuv.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://ojr.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mjj.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://htj.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wmh.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://utz.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uys.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hlj.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ipp.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pns.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://amy.ppjwa.cn

[E06] 替换子串
来源：http://cpu.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hsw.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://ydb.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufw.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://tnp.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tti.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wpz.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wwr.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://oxv.fzhhl.top

[E07] 按分隔符拆分
来源：http://mlz.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tdb.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jsi.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dsk.hcnkem.com

TS:   s.split(",")
来源：http://vnm.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://rpc.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lfw.zhengqikj.top


<!-- 参考信息 -->