代发 wailian999

Java: list.add(4);
来源：https://jd.zhonguo1118.cn

Go:   arr = append(arr, 4)
来源：https://gz.zhonguo5118.cn

Ruby: arr << 4; arr.push(5)
来源：https://cj.zhonguo2118.cn

C#:   list.Add(4);
来源：https://rh.zhonguo5118.cn

[D03] 在指定位置插入元素
来源：https://im.zhonguo1118.cn

Py:   arr.insert(0, 0)
来源：https://fb.zhonguo6118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://dd.zhonguo5118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://jg.zhonguo7118.cn

TS:   arr.splice(0, 0, 0);
来源：https://jk.zhonguo2118.cn

Java: list.add(0, 0);
来源：https://mf.zhonguo5118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://eh.zhonguo2118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://qz.zhonguo1118.cn

C#:   list.Insert(0, 0);
来源：https://ye.zhonguo5118.cn

[D04] 删除元素
来源：https://dg.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://el.zhonguo1118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://cp.zhonguo2118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://hm.zhonguo4118.cn

TS:   arr.splice(0, 1);
来源：https://zj.zhonguo8118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://fl.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://in.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://sx.zhonguo8118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://jc.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://ta.zhonguo1118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://lg.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://lx.zhonguo6118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://dy.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://mc.zhonguo6118.cn

Java: list.get(0); list.set(0, 9);
来源：https://dr.zhonguo8118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ji.zhonguo6118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://zi.zhonguo1118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://me.zhonguo4118.cn

[D06] 数组长度
来源：https://my.zhonguo3118.cn

Py:   len(arr)
来源：https://cq.zhonguo6118.cn

PHP:  count($arr);
来源：https://nx.zhonguo1118.cn

JS:   arr.length
来源：https://vh.zhonguo5118.cn

TS:   arr.length
来源：https://ws.zhonguo6118.cn

Java: list.size();
来源：https://gk.zhonguo2118.cn

Go:   len(arr)
来源：https://ix.zhonguo5118.cn

Ruby: arr.length; arr.size
来源：https://fx.zhonguo5118.cn

C#:   list.Count;
来源：https://lb.zhonguo1118.cn

[D07] 切片 / 取子数组
来源：https://md.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://vv.zhonguo6118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://rv.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://ix.zhonguo6118.cn

TS:   arr.slice(1, 4);
来源：https://zk.zhonguo5118.cn

Java: list.subList(1, 4);
来源：https://xu.zhonguo4118.cn

Go:   arr[1:4]
来源：https://ga.zhonguo4118.cn

Ruby: arr[1, 3]
来源：https://xv.zhonguo4118.cn

C#:   list.GetRange(1, 3);
来源：https://sk.zhonguo2118.cn

[D08] 合并两个数组
来源：https://eq.zhonguo6118.cn

Py:   a + b;  a.extend(b)
来源：https://qk.zhonguo2118.cn

PHP:  array_merge($a, $b);
来源：https://bg.zhonguo5118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ni.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://oa.zhonguo6118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://do.zhonguo4118.cn

Go:   append(a, b...)
来源：https://be.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://qx.zhonguo6118.cn

C#:   a.Concat(b).ToList()
来源：https://ew.zhonguo4118.cn

[D09] 排序（升序）
来源：https://qy.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://zq.zhonguo2118.cn

PHP:  sort($arr);
来源：https://hw.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://qa.zhonguo2118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://yt.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://ed.zhonguo8118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://yt.zhonguo6118.cn

Ruby: arr.sort
来源：https://yk.zhonguo3118.cn

C#:   list.Sort();
来源：https://mt.zhonguo1118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://mx.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://wd.zhonguo6118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://qr.zhonguo4118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://so.zhonguo8118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://du.zhonguo6118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://uz.zhonguo4118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://ap.zhonguo1118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://aa.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://uk.zhonguo3118.cn

[D11] 反转数组
来源：https://io.zhonguo5118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://tv.zhonguo5118.cn

PHP:  array_reverse($arr);
来源：https://eg.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://ay.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://gy.zhonguo8118.cn

Java: Collections.reverse(list);
来源：https://ze.zhonguo8118.cn

Go:   slices.Reverse(arr)
来源：https://lj.zhonguo6118.cn

Ruby: arr.reverse
来源：https://vi.zhonguo6118.cn

C#:   list.Reverse();
来源：https://tg.zhonguo7118.cn

[D12] 查找元素下标
来源：https://xh.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://cj.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://wp.zhonguo8118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://zq.zhonguo1118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://gv.zhonguo7118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://jc.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://kl.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://wx.zhonguo6118.cn

C#:   list.IndexOf(x);
来源：https://bh.zhonguo6118.cn

[D13] 过滤（保留满足条件的）
来源：https://ka.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://hm.zhonguo7118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://io.zhonguo8118.cn

JS:   arr.filter(x => x > 3)
来源：https://kq.zhonguo2118.cn

TS:   arr.filter(x => x > 3)
来源：https://hm.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://hj.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://bu.zhonguo2118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://jb.zhonguo8118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ab.zhonguo3118.cn

[D14] 映射转换（每个元素变形）
来源：https://vq.zhonguo6118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://ah.zhonguo7118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://qc.zhonguo3118.cn

JS:   arr.map(x => x * 2)
来源：https://ww.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://gn.zhonguo3118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://hg.zhonguo6118.cn

Go:   // 手写循环
来源：https://jd.zhonguo4118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://mn.zhonguo8118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://cz.zhonguo6118.cn

[D15] 去重
来源：https://co.zhonguo3118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://zx.zhonguo3118.cn

PHP:  array_unique($arr);
来源：https://ph.zhonguo3118.cn

JS:   [...new Set(arr)]
来源：https://ty.zhonguo8118.cn

TS:   [...new Set(arr)]
来源：https://ra.zhonguo1118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://bz.zhonguo7118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://vm.zhonguo6118.cn

Ruby: arr.uniq
来源：https://kg.zhonguo4118.cn

C#:   list.Distinct().ToList()
来源：https://ux.zhonguo7118.cn

[D16] 求和与平均值
来源：https://at.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://xp.zhonguo5118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://fw.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://nj.zhonguo8118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://bo.zhonguo8118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://vz.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://sn.zhonguo6118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://lz.zhonguo5118.cn

C#:   list.Sum();  list.Average()
来源：https://ep.zhonguo7118.cn

[D17] 最大值与最小值
来源：https://ko.zhonguo4118.cn

Py:   max(arr);  min(arr)
来源：https://hz.zhonguo4118.cn

PHP:  max($arr);  min($arr);
来源：https://rv.zhonguo5118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://fl.zhonguo7118.cn

TS:   Math.max(...arr);
来源：https://wn.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://gy.zhonguo7118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://tx.zhonguo8118.cn

Ruby: arr.max;  arr.min
来源：https://pj.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://yp.zhonguo8118.cn

[D18] 扁平化嵌套数组
来源：https://po.zhonguo2118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ja.zhonguo5118.cn

PHP:  array_merge(...$nested);
来源：https://ay.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://dm.zhonguo4118.cn

TS:   nested.flat();
来源：https://pi.zhonguo6118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ff.zhonguo3118.cn

Go:   // 手写双层循环
来源：https://iq.zhonguo5118.cn

Ruby: nested.flatten
来源：https://qk.zhonguo2118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://md.zhonguo4118.cn

[D19] 按字段分组
来源：https://cr.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://yz.zhonguo5118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://rx.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://qx.zhonguo8118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://jh.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ef.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://tf.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ur.zhonguo3118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://kj.zhonguo3118.cn

[D20] 统计每个元素出现次数
来源：https://gf.zhonguo1118.cn

Py:   Counter(arr)
来源：https://pq.zhonguo1118.cn

PHP:  array_count_values($arr);
来源：https://ag.zhonguo6118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://bs.zhonguo7118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://hm.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://ib.zhonguo4118.cn

Go:   // 手写 map[T]int
来源：https://uu.zhonguo2118.cn

Ruby: arr.tally
来源：https://az.zhonguo3118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://cs.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://fb.zhonguo8118.cn

Py:   x in arr
来源：https://lq.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://te.zhonguo6118.cn

JS:   arr.includes(x)
来源：https://xc.zhonguo1118.cn

TS:   arr.includes(x)
来源：https://co.zhonguo3118.cn

Java: list.contains(x)
来源：https://cm.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://tn.zhonguo5118.cn

Ruby: arr.include?(x)
来源：https://ez.zhonguo8118.cn

C#:   list.Contains(x)
来源：https://ok.zhonguo4118.cn

[D22] 复制数组（避免共享引用）
来源：https://wy.zhonguo4118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ml.zhonguo2118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://zw.zhonguo8118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://qn.zhonguo3118.cn

TS:   [...arr];
来源：https://yz.zhonguo8118.cn

Java: new ArrayList<>(list);
来源：https://ve.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://sp.zhonguo5118.cn

Ruby: arr.dup;  arr.clone
来源：https://sb.zhonguo7118.cn

C#:   new List<int>(list);
来源：https://mi.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://cf.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://jj.zhonguo3118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://uz.zhonguo4118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://wg.zhonguo5118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://hq.zhonguo2118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://ig.zhonguo1118.cn

Go:   // 手写循环
来源：https://rp.zhonguo7118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://jl.zhonguo7118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://jz.zhonguo2118.cn

[D24] 字典 / Map 基本操作
来源：https://yh.zhonguo3118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://zd.zhonguo7118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://nn.zhonguo3118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://iz.zhonguo8118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://mc.zhonguo1118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://vv.zhonguo4118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://kv.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://my.zhonguo3118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://lr.zhonguo7118.cn

[D25] Set 集合去重与交并差
来源：https://eg.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://uh.zhonguo8118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://sh.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://aq.zhonguo4118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ah.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://cs.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://ul.zhonguo3118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://vl.zhonguo2118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://vj.zhonguo5118.cn

[D26] 数组转字符串
来源：https://du.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://qk.zhonguo6118.cn

PHP:  implode(", ", $arr);
来源：https://py.zhonguo1118.cn

JS:   arr.join(", ")
来源：https://yv.zhonguo8118.cn

TS:   arr.join(", ")
来源：https://ik.zhonguo1118.cn

Java: String.join(", ", list)
来源：https://ms.zhonguo1118.cn

Go:   strings.Join(strs, ", ")
来源：https://wh.zhonguo4118.cn

Ruby: arr.join(", ")
来源：https://ic.zhonguo6118.cn

C#:   string.Join(", ", list)
来源：https://gb.zhonguo6118.cn

================================================================================
来源：https://lh.zhonguo4118.cn

E. 字符串处理
来源：https://jj.zhonguo7118.cn

================================================================================
来源：https://gn.zhonguo5118.cn

[E01] 拼接字符串
来源：https://za.zhonguo2118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://tc.zhonguo3118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://ph.zhonguo2118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://bm.zhonguo4118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://fj.zhonguo7118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://tj.zhonguo2118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://kx.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://am.zhonguo3118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://um.zhonguo5118.cn

[E02] 重复字符串
来源：https://pu.zhonguo4118.cn

Py:   "ab" * 3
来源：https://xl.zhonguo8118.cn

PHP:  str_repeat("ab", 3);
来源：https://lk.zhonguo3118.cn

JS:   "ab".repeat(3)
来源：https://mw.zhonguo7118.cn

TS:   "ab".repeat(3)
来源：https://tn.zhonguo4118.cn

Java: "ab".repeat(3)
来源：https://hp.zhonguo3118.cn

Go:   strings.Repeat("ab", 3)
来源：https://wy.zhonguo4118.cn

Ruby: "ab" * 3
来源：https://vf.zhonguo7118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://mf.zhonguo7118.cn

[E03] 截取子串
来源：https://tn.zhonguo5118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://il.zhonguo8118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://de.zhonguo8118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://jr.zhonguo1118.cn

TS:   s.slice(1, 4)
来源：https://iu.zhonguo5118.cn

Java: s.substring(1, 4)
来源：https://kd.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://rs.zhonguo5118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://vr.zhonguo6118.cn

C#:   s.Substring(1, 3)
来源：https://ga.zhonguo3118.cn

[E04] 查找子串位置
来源：https://ut.zhonguo8118.cn

Py:   s.find("x");  s.index("x")
来源：https://su.zhonguo5118.cn

PHP:  strpos($s, "x");
来源：https://dc.zhonguo4118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://ur.zhonguo5118.cn

TS:   s.indexOf("x")
来源：https://se.zhonguo1118.cn

Java: s.indexOf("x")
来源：https://xi.zhonguo1118.cn

Go:   strings.Index(s, "x")
来源：https://nq.zhonguo4118.cn

Ruby: s.index("x")
来源：https://kl.zhonguo8118.cn

C#:   s.IndexOf("x")
来源：https://zf.zhonguo3118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://mb.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://mv.zhonguo8118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://zf.zhonguo7118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://xp.zhonguo1118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://bt.zhonguo1118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ct.zhonguo7118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://bf.zhonguo2118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://uy.zhonguo4118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://ay.zhonguo2118.cn

[E06] 替换子串
来源：https://tz.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://on.zhonguo5118.cn

PHP:  str_replace("a", "b", $s);
来源：https://el.zhonguo6118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://bw.zhonguo8118.cn

TS:   s.replaceAll("a", "b")
来源：https://pb.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://yj.zhonguo7118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://pf.zhonguo7118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://cg.zhonguo8118.cn

C#:   s.Replace("a", "b")
来源：https://cl.zhonguo5118.cn

[E07] 按分隔符拆分
来源：https://bs.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://pa.zhonguo8118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://wk.zhonguo3118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://cp.zhonguo1118.cn

TS:   s.split(",")
来源：https://gd.zhonguo2118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://lu.zhonguo4118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ym.zhonguo2118.cn

Ruby: s.split(",");  s.split
来源：https://uf.zhonguo3118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://jg.zhonguo4118.cn

[E08] 数组按分隔符合并
来源：https://oo.zhonguo4118.cn

Py:   ",".join(items)
来源：https://vp.zhonguo1118.cn

PHP:  implode(",", $items);
来源：https://se.zhonguo2118.cn

JS:   items.join(",")
来源：https://zv.zhonguo4118.cn

TS:   items.join(",")
来源：https://dd.zhonguo3118.cn

Java: String.join(",", items)
来源：https://hj.zhonguo8118.cn

Go:   strings.Join(items, ",")
来源：https://bp.zhonguo7118.cn

Ruby: items.join(",")
来源：https://dy.zhonguo1118.cn

C#:   string.Join(",", items)
来源：https://mq.zhonguo8118.cn

[E09] 去除所有空白字符
来源：https://zo.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://tf.zhonguo6118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://dn.zhonguo8118.cn

JS:   s.replace(/\s+/g, "")
来源：https://xd.zhonguo4118.cn

TS:   s.replace(/\s+/g, "")
来源：https://aa.zhonguo2118.cn


<!-- 参考信息 -->