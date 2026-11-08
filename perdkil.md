代发 wailian999

Go:   // 无重载：用不同函数名
来源：https://vd.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://ai.zhonguo7118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://df.zhonguo7118.cn

================================================================================
来源：https://te.zhonguo4118.cn

D. 数组 / 列表 / 集合
来源：https://if.zhonguo5118.cn

================================================================================
来源：https://nv.zhonguo2118.cn

[D01] 创建数组 / 列表
来源：https://yd.zhonguo8118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://ge.zhonguo4118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://lv.zhonguo4118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://pw.zhonguo4118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://lw.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://fc.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://xg.zhonguo5118.cn

Ruby: arr = [1, 2, 3]
来源：https://yt.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://ys.zhonguo5118.cn

[D02] 追加元素到末尾
来源：https://gn.zhonguo6118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://cc.zhonguo7118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://dq.zhonguo1118.cn

JS:   arr.push(4);
来源：https://wo.zhonguo1118.cn

TS:   arr.push(4);
来源：https://jk.zhonguo8118.cn

Java: list.add(4);
来源：https://kz.zhonguo6118.cn

Go:   arr = append(arr, 4)
来源：https://ar.zhonguo2118.cn

Ruby: arr << 4; arr.push(5)
来源：https://lb.zhonguo7118.cn

C#:   list.Add(4);
来源：https://hl.zhonguo6118.cn

[D03] 在指定位置插入元素
来源：https://xu.zhonguo4118.cn

Py:   arr.insert(0, 0)
来源：https://wy.zhonguo3118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://jy.zhonguo8118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://vk.zhonguo5118.cn

TS:   arr.splice(0, 0, 0);
来源：https://kg.zhonguo1118.cn

Java: list.add(0, 0);
来源：https://se.zhonguo1118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://so.zhonguo2118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://ue.zhonguo8118.cn

C#:   list.Insert(0, 0);
来源：https://ja.zhonguo4118.cn

[D04] 删除元素
来源：https://xk.zhonguo1118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://xd.zhonguo7118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ai.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://zx.zhonguo6118.cn

TS:   arr.splice(0, 1);
来源：https://tk.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://xm.zhonguo8118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ql.zhonguo7118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://oj.zhonguo6118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://jh.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://hq.zhonguo6118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://mq.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://rw.zhonguo8118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://ca.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://dp.zhonguo5118.cn

Java: list.get(0); list.set(0, 9);
来源：https://vs.zhonguo5118.cn

Go:   arr[0]; arr[0] = 9
来源：https://zy.zhonguo6118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://vw.zhonguo8118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://mc.zhonguo6118.cn

[D06] 数组长度
来源：https://lg.zhonguo5118.cn

Py:   len(arr)
来源：https://ca.zhonguo4118.cn

PHP:  count($arr);
来源：https://by.zhonguo4118.cn

JS:   arr.length
来源：https://po.zhonguo2118.cn

TS:   arr.length
来源：https://tt.zhonguo3118.cn

Java: list.size();
来源：https://lj.zhonguo8118.cn

Go:   len(arr)
来源：https://ry.zhonguo4118.cn

Ruby: arr.length; arr.size
来源：https://py.zhonguo4118.cn

C#:   list.Count;
来源：https://bn.zhonguo2118.cn

[D07] 切片 / 取子数组
来源：https://jf.zhonguo3118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://qg.zhonguo5118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://fv.zhonguo8118.cn

JS:   arr.slice(1, 4);
来源：https://be.zhonguo8118.cn

TS:   arr.slice(1, 4);
来源：https://hz.zhonguo2118.cn

Java: list.subList(1, 4);
来源：https://ll.zhonguo4118.cn

Go:   arr[1:4]
来源：https://tu.zhonguo1118.cn

Ruby: arr[1, 3]
来源：https://bj.zhonguo4118.cn

C#:   list.GetRange(1, 3);
来源：https://sf.zhonguo5118.cn

[D08] 合并两个数组
来源：https://ps.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://ev.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://fv.zhonguo5118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://dy.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://rl.zhonguo1118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ij.zhonguo7118.cn

Go:   append(a, b...)
来源：https://fe.zhonguo3118.cn

Ruby: a + b;  a.concat(b)
来源：https://ei.zhonguo5118.cn

C#:   a.Concat(b).ToList()
来源：https://pc.zhonguo3118.cn

[D09] 排序（升序）
来源：https://fq.zhonguo2118.cn

Py:   sorted(arr);  arr.sort()
来源：https://rz.zhonguo3118.cn

PHP:  sort($arr);
来源：https://cb.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://zm.zhonguo8118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ce.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://jn.zhonguo3118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://yg.zhonguo2118.cn

Ruby: arr.sort
来源：https://ba.zhonguo4118.cn

C#:   list.Sort();
来源：https://kz.zhonguo5118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://ya.zhonguo2118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://yo.zhonguo7118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://fe.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://hf.zhonguo5118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://yl.zhonguo1118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://hg.zhonguo7118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://zv.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://hr.zhonguo7118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://eq.zhonguo7118.cn

[D11] 反转数组
来源：https://vb.zhonguo4118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://zc.zhonguo2118.cn

PHP:  array_reverse($arr);
来源：https://hy.zhonguo3118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://at.zhonguo4118.cn

TS:   [...arr].reverse();
来源：https://io.zhonguo5118.cn

Java: Collections.reverse(list);
来源：https://dp.zhonguo4118.cn

Go:   slices.Reverse(arr)
来源：https://lh.zhonguo4118.cn

Ruby: arr.reverse
来源：https://os.zhonguo6118.cn

C#:   list.Reverse();
来源：https://yo.zhonguo4118.cn

[D12] 查找元素下标
来源：https://ob.zhonguo2118.cn

Py:   arr.index(x);  x in arr
来源：https://pr.zhonguo5118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://hz.zhonguo3118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://fl.zhonguo7118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://rg.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://st.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://ez.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://lz.zhonguo8118.cn

C#:   list.IndexOf(x);
来源：https://nu.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://uj.zhonguo8118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://pa.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://my.zhonguo1118.cn

JS:   arr.filter(x => x > 3)
来源：https://cz.zhonguo8118.cn

TS:   arr.filter(x => x > 3)
来源：https://mg.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://eq.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://uo.zhonguo6118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://pq.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ez.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://zp.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://at.zhonguo7118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://cy.zhonguo7118.cn

JS:   arr.map(x => x * 2)
来源：https://tz.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://rr.zhonguo4118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://hr.zhonguo7118.cn

Go:   // 手写循环
来源：https://tw.zhonguo3118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://pq.zhonguo8118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://jc.zhonguo3118.cn

[D15] 去重
来源：https://li.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ah.zhonguo6118.cn

PHP:  array_unique($arr);
来源：https://rt.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://zq.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://wn.zhonguo6118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://up.zhonguo7118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ix.zhonguo1118.cn

Ruby: arr.uniq
来源：https://wc.zhonguo8118.cn

C#:   list.Distinct().ToList()
来源：https://yg.zhonguo4118.cn

[D16] 求和与平均值
来源：https://fj.zhonguo2118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://lg.zhonguo8118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://rn.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://zs.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://si.zhonguo4118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://ny.zhonguo3118.cn

Go:   // 手写循环累加
来源：https://zx.zhonguo2118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ol.zhonguo4118.cn

C#:   list.Sum();  list.Average()
来源：https://fj.zhonguo5118.cn

[D17] 最大值与最小值
来源：https://oe.zhonguo4118.cn

Py:   max(arr);  min(arr)
来源：https://ps.zhonguo3118.cn

PHP:  max($arr);  min($arr);
来源：https://xr.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://lz.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://qq.zhonguo5118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://fy.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://mo.zhonguo7118.cn

Ruby: arr.max;  arr.min
来源：https://kt.zhonguo2118.cn

C#:   list.Max();  list.Min()
来源：https://gx.zhonguo2118.cn

[D18] 扁平化嵌套数组
来源：https://cl.zhonguo1118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://cj.zhonguo1118.cn

PHP:  array_merge(...$nested);
来源：https://db.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://nk.zhonguo6118.cn

TS:   nested.flat();
来源：https://ch.zhonguo1118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ao.zhonguo2118.cn

Go:   // 手写双层循环
来源：https://nn.zhonguo5118.cn

Ruby: nested.flatten
来源：https://hp.zhonguo4118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://ty.zhonguo3118.cn

[D19] 按字段分组
来源：https://wp.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://wh.zhonguo3118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://lh.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://mr.zhonguo4118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://jx.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ev.zhonguo8118.cn

Go:   // 手写 map[string][]T
来源：https://mk.zhonguo8118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://eh.zhonguo1118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://qh.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://oh.zhonguo2118.cn

Py:   Counter(arr)
来源：https://iw.zhonguo4118.cn

PHP:  array_count_values($arr);
来源：https://xu.zhonguo6118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://la.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://dk.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://ju.zhonguo2118.cn

Go:   // 手写 map[T]int
来源：https://po.zhonguo1118.cn

Ruby: arr.tally
来源：https://el.zhonguo2118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://gr.zhonguo1118.cn

[D21] 判断是否包含某元素
来源：https://yf.zhonguo1118.cn

Py:   x in arr
来源：https://sf.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://dv.zhonguo4118.cn

JS:   arr.includes(x)
来源：https://am.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://gl.zhonguo1118.cn

Java: list.contains(x)
来源：https://ue.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://ec.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://fd.zhonguo4118.cn

C#:   list.Contains(x)
来源：https://ev.zhonguo8118.cn

[D22] 复制数组（避免共享引用）
来源：https://az.zhonguo3118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://mq.zhonguo4118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ki.zhonguo6118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://en.zhonguo8118.cn

TS:   [...arr];
来源：https://st.zhonguo5118.cn

Java: new ArrayList<>(list);
来源：https://xd.zhonguo7118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://vj.zhonguo4118.cn

Ruby: arr.dup;  arr.clone
来源：https://ol.zhonguo5118.cn

C#:   new List<int>(list);
来源：https://eb.zhonguo4118.cn

[D23] reduce 累积计算
来源：https://xu.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ir.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://ic.zhonguo1118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://qc.zhonguo2118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ws.zhonguo1118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://rg.zhonguo7118.cn

Go:   // 手写循环
来源：https://pk.zhonguo3118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://bw.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://pc.zhonguo7118.cn

[D24] 字典 / Map 基本操作
来源：https://wm.zhonguo8118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://pz.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://mt.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://vp.zhonguo5118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://tx.zhonguo8118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://jq.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://xa.zhonguo3118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://pd.zhonguo4118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://is.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://ey.zhonguo7118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://lx.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://sl.zhonguo4118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://xl.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://wz.zhonguo8118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://kk.zhonguo8118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://kv.zhonguo4118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://ln.zhonguo6118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://au.zhonguo6118.cn

[D26] 数组转字符串
来源：https://xe.zhonguo2118.cn

Py:   ", ".join(map(str, arr))
来源：https://hj.zhonguo4118.cn

PHP:  implode(", ", $arr);
来源：https://tq.zhonguo5118.cn

JS:   arr.join(", ")
来源：https://yu.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://lj.zhonguo4118.cn

Java: String.join(", ", list)
来源：https://va.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://ex.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://ky.zhonguo4118.cn

C#:   string.Join(", ", list)
来源：https://pk.zhonguo3118.cn

================================================================================
来源：https://qb.zhonguo7118.cn

E. 字符串处理
来源：https://af.zhonguo3118.cn

================================================================================
来源：https://sj.zhonguo3118.cn

[E01] 拼接字符串
来源：https://vf.zhonguo6118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://yi.zhonguo7118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://fz.zhonguo2118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://sk.zhonguo8118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://cz.zhonguo8118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://jj.zhonguo7118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://rb.zhonguo7118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://wx.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://rx.zhonguo4118.cn

[E02] 重复字符串
来源：https://xx.zhonguo5118.cn

Py:   "ab" * 3
来源：https://tz.zhonguo7118.cn

PHP:  str_repeat("ab", 3);
来源：https://dc.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://oh.zhonguo5118.cn

TS:   "ab".repeat(3)
来源：https://rz.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://od.zhonguo4118.cn

Go:   strings.Repeat("ab", 3)
来源：https://bp.zhonguo4118.cn

Ruby: "ab" * 3
来源：https://oy.zhonguo7118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://vj.zhonguo2118.cn

[E03] 截取子串
来源：https://el.zhonguo1118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://xh.zhonguo1118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://qb.zhonguo6118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://iy.zhonguo2118.cn

TS:   s.slice(1, 4)
来源：https://fm.zhonguo5118.cn

Java: s.substring(1, 4)
来源：https://hv.zhonguo7118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://zv.zhonguo4118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://fl.zhonguo5118.cn

C#:   s.Substring(1, 3)
来源：https://fp.zhonguo7118.cn

[E04] 查找子串位置
来源：https://bz.zhonguo8118.cn

Py:   s.find("x");  s.index("x")
来源：https://ph.zhonguo1118.cn

PHP:  strpos($s, "x");
来源：https://ia.zhonguo3118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://sg.zhonguo6118.cn

TS:   s.indexOf("x")
来源：https://jr.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://pf.zhonguo3118.cn

Go:   strings.Index(s, "x")
来源：https://tp.zhonguo1118.cn

Ruby: s.index("x")
来源：https://sw.zhonguo5118.cn

C#:   s.IndexOf("x")
来源：https://ve.zhonguo3118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://hi.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ui.zhonguo3118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://rn.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://pt.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://zj.zhonguo1118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://zb.zhonguo4118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://fl.zhonguo5118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://sn.zhonguo1118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://js.zhonguo3118.cn

[E06] 替换子串
来源：https://mt.zhonguo8118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://dz.zhonguo5118.cn

PHP:  str_replace("a", "b", $s);
来源：https://xq.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://vj.zhonguo8118.cn

TS:   s.replaceAll("a", "b")
来源：https://ua.zhonguo8118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://me.zhonguo2118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://it.zhonguo7118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://pa.zhonguo1118.cn

C#:   s.Replace("a", "b")
来源：https://yo.zhonguo3118.cn

[E07] 按分隔符拆分
来源：https://wg.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://ak.zhonguo7118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://wd.zhonguo5118.cn


<!-- 参考信息 -->