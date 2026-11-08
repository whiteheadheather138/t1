代发 wailian999

PHP:  // 无重载
来源：https://xd.zhonguo7118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://al.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://yk.zhonguo8118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://tc.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://gq.zhonguo4118.cn

Ruby: # 无重载：靠动态参数
来源：https://jq.zhonguo8118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://jb.zhonguo2118.cn

================================================================================
来源：https://gf.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://gr.zhonguo8118.cn

================================================================================
来源：https://vj.zhonguo2118.cn

[D01] 创建数组 / 列表
来源：https://kb.zhonguo8118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://km.zhonguo6118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://pj.zhonguo4118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://ay.zhonguo8118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://rb.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://jz.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://ev.zhonguo2118.cn

Ruby: arr = [1, 2, 3]
来源：https://wy.zhonguo3118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://no.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://zb.zhonguo4118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://gi.zhonguo6118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://in.zhonguo2118.cn

JS:   arr.push(4);
来源：https://im.zhonguo1118.cn

TS:   arr.push(4);
来源：https://zl.zhonguo1118.cn

Java: list.add(4);
来源：https://zb.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://pj.zhonguo3118.cn

Ruby: arr << 4; arr.push(5)
来源：https://rm.zhonguo4118.cn

C#:   list.Add(4);
来源：https://rm.zhonguo4118.cn

[D03] 在指定位置插入元素
来源：https://ck.zhonguo3118.cn

Py:   arr.insert(0, 0)
来源：https://xp.zhonguo3118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://ua.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://sc.zhonguo7118.cn

TS:   arr.splice(0, 0, 0);
来源：https://ca.zhonguo5118.cn

Java: list.add(0, 0);
来源：https://mn.zhonguo6118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://oz.zhonguo8118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://ls.zhonguo4118.cn

C#:   list.Insert(0, 0);
来源：https://nf.zhonguo7118.cn

[D04] 删除元素
来源：https://mx.zhonguo4118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://rl.zhonguo7118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://tn.zhonguo1118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://ub.zhonguo4118.cn

TS:   arr.splice(0, 1);
来源：https://mu.zhonguo7118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://wj.zhonguo6118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ws.zhonguo1118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ql.zhonguo4118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://gg.zhonguo4118.cn

[D05] 访问与修改元素
来源：https://yb.zhonguo4118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://ef.zhonguo7118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://vn.zhonguo2118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://xz.zhonguo2118.cn

TS:   arr[0]; arr.at(-1);
来源：https://od.zhonguo3118.cn

Java: list.get(0); list.set(0, 9);
来源：https://bv.zhonguo8118.cn

Go:   arr[0]; arr[0] = 9
来源：https://zu.zhonguo8118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://uo.zhonguo8118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://ug.zhonguo8118.cn

[D06] 数组长度
来源：https://ap.zhonguo7118.cn

Py:   len(arr)
来源：https://kb.zhonguo5118.cn

PHP:  count($arr);
来源：https://dd.zhonguo1118.cn

JS:   arr.length
来源：https://gk.zhonguo8118.cn

TS:   arr.length
来源：https://mm.zhonguo1118.cn

Java: list.size();
来源：https://yq.zhonguo2118.cn

Go:   len(arr)
来源：https://vu.zhonguo4118.cn

Ruby: arr.length; arr.size
来源：https://hh.zhonguo6118.cn

C#:   list.Count;
来源：https://qm.zhonguo7118.cn

[D07] 切片 / 取子数组
来源：https://xv.zhonguo3118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://xn.zhonguo5118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://jq.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://to.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://au.zhonguo5118.cn

Java: list.subList(1, 4);
来源：https://jf.zhonguo4118.cn

Go:   arr[1:4]
来源：https://hy.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://th.zhonguo5118.cn

C#:   list.GetRange(1, 3);
来源：https://fo.zhonguo2118.cn

[D08] 合并两个数组
来源：https://ro.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://wv.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://kz.zhonguo4118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://xt.zhonguo6118.cn

TS:   [...a, ...b];
来源：https://wj.zhonguo2118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://do.zhonguo3118.cn

Go:   append(a, b...)
来源：https://te.zhonguo6118.cn

Ruby: a + b;  a.concat(b)
来源：https://az.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://bg.zhonguo1118.cn

[D09] 排序（升序）
来源：https://vd.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://ps.zhonguo5118.cn

PHP:  sort($arr);
来源：https://eb.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://gb.zhonguo4118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ml.zhonguo4118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://cj.zhonguo6118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://vw.zhonguo2118.cn

Ruby: arr.sort
来源：https://xv.zhonguo8118.cn

C#:   list.Sort();
来源：https://pi.zhonguo2118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://di.zhonguo5118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://ug.zhonguo5118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ht.zhonguo3118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://jw.zhonguo4118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://vi.zhonguo8118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://af.zhonguo2118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://zg.zhonguo8118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://us.zhonguo5118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://kt.zhonguo6118.cn

[D11] 反转数组
来源：https://ew.zhonguo1118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://sz.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://lt.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://ys.zhonguo4118.cn

TS:   [...arr].reverse();
来源：https://pi.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://km.zhonguo4118.cn

Go:   slices.Reverse(arr)
来源：https://zr.zhonguo7118.cn

Ruby: arr.reverse
来源：https://le.zhonguo2118.cn

C#:   list.Reverse();
来源：https://im.zhonguo4118.cn

[D12] 查找元素下标
来源：https://yw.zhonguo6118.cn

Py:   arr.index(x);  x in arr
来源：https://pq.zhonguo8118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://fm.zhonguo5118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://wu.zhonguo1118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jm.zhonguo1118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://xn.zhonguo6118.cn

Go:   slices.Index(arr, x)
来源：https://qn.zhonguo3118.cn

Ruby: arr.index(x)
来源：https://oj.zhonguo2118.cn

C#:   list.IndexOf(x);
来源：https://zw.zhonguo4118.cn

[D13] 过滤（保留满足条件的）
来源：https://nd.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://ml.zhonguo3118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://cz.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://ji.zhonguo6118.cn

TS:   arr.filter(x => x > 3)
来源：https://wf.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://mu.zhonguo6118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://gz.zhonguo6118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ou.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://bs.zhonguo5118.cn

[D14] 映射转换（每个元素变形）
来源：https://db.zhonguo4118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://rd.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://it.zhonguo4118.cn

JS:   arr.map(x => x * 2)
来源：https://rx.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://pi.zhonguo7118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://dt.zhonguo7118.cn

Go:   // 手写循环
来源：https://ev.zhonguo5118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://ts.zhonguo7118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://si.zhonguo6118.cn

[D15] 去重
来源：https://bo.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://zd.zhonguo2118.cn

PHP:  array_unique($arr);
来源：https://jv.zhonguo6118.cn

JS:   [...new Set(arr)]
来源：https://li.zhonguo4118.cn

TS:   [...new Set(arr)]
来源：https://kq.zhonguo8118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://oy.zhonguo5118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://tj.zhonguo5118.cn

Ruby: arr.uniq
来源：https://df.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://gp.zhonguo6118.cn

[D16] 求和与平均值
来源：https://nn.zhonguo2118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://jc.zhonguo1118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://px.zhonguo5118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://ta.zhonguo1118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://qr.zhonguo3118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://rn.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://wa.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://so.zhonguo4118.cn

C#:   list.Sum();  list.Average()
来源：https://hr.zhonguo3118.cn

[D17] 最大值与最小值
来源：https://og.zhonguo3118.cn

Py:   max(arr);  min(arr)
来源：https://rc.zhonguo1118.cn

PHP:  max($arr);  min($arr);
来源：https://zw.zhonguo8118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://zc.zhonguo4118.cn

TS:   Math.max(...arr);
来源：https://wl.zhonguo7118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://yi.zhonguo8118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://vt.zhonguo8118.cn

Ruby: arr.max;  arr.min
来源：https://mi.zhonguo2118.cn

C#:   list.Max();  list.Min()
来源：https://vh.zhonguo2118.cn

[D18] 扁平化嵌套数组
来源：https://hl.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://pq.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://gi.zhonguo4118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://ci.zhonguo6118.cn

TS:   nested.flat();
来源：https://jq.zhonguo5118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://bj.zhonguo1118.cn

Go:   // 手写双层循环
来源：https://jt.zhonguo5118.cn

Ruby: nested.flatten
来源：https://ik.zhonguo3118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://ey.zhonguo3118.cn

[D19] 按字段分组
来源：https://ww.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://lf.zhonguo3118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://jw.zhonguo3118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://fe.zhonguo4118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://kg.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://di.zhonguo6118.cn

Go:   // 手写 map[string][]T
来源：https://dw.zhonguo5118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://it.zhonguo3118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://rr.zhonguo3118.cn

[D20] 统计每个元素出现次数
来源：https://wm.zhonguo6118.cn

Py:   Counter(arr)
来源：https://uq.zhonguo4118.cn

PHP:  array_count_values($arr);
来源：https://xd.zhonguo7118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://rb.zhonguo1118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://lw.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://pg.zhonguo3118.cn

Go:   // 手写 map[T]int
来源：https://ki.zhonguo6118.cn

Ruby: arr.tally
来源：https://bp.zhonguo7118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://cv.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://mw.zhonguo5118.cn

Py:   x in arr
来源：https://bn.zhonguo2118.cn

PHP:  in_array($x, $arr, true);
来源：https://sm.zhonguo6118.cn

JS:   arr.includes(x)
来源：https://bb.zhonguo4118.cn

TS:   arr.includes(x)
来源：https://gg.zhonguo3118.cn

Java: list.contains(x)
来源：https://ax.zhonguo3118.cn

Go:   slices.Contains(arr, x)
来源：https://qb.zhonguo1118.cn

Ruby: arr.include?(x)
来源：https://zj.zhonguo8118.cn

C#:   list.Contains(x)
来源：https://eu.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://pa.zhonguo6118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ev.zhonguo8118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://zp.zhonguo3118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://pb.zhonguo2118.cn

TS:   [...arr];
来源：https://ny.zhonguo8118.cn

Java: new ArrayList<>(list);
来源：https://yw.zhonguo2118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://ky.zhonguo2118.cn

Ruby: arr.dup;  arr.clone
来源：https://ie.zhonguo2118.cn

C#:   new List<int>(list);
来源：https://lv.zhonguo5118.cn

[D23] reduce 累积计算
来源：https://ah.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://lk.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://bp.zhonguo2118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://mj.zhonguo5118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://zu.zhonguo7118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://cs.zhonguo7118.cn

Go:   // 手写循环
来源：https://ud.zhonguo3118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://tz.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://xu.zhonguo1118.cn

[D24] 字典 / Map 基本操作
来源：https://oo.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://sn.zhonguo3118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://zj.zhonguo4118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://ec.zhonguo7118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://px.zhonguo5118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://oy.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://rj.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ri.zhonguo6118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://xf.zhonguo2118.cn

[D25] Set 集合去重与交并差
来源：https://ov.zhonguo1118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://sz.zhonguo4118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://lq.zhonguo8118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://mu.zhonguo5118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://st.zhonguo6118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://ig.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://tr.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://fs.zhonguo1118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://pr.zhonguo7118.cn

[D26] 数组转字符串
来源：https://xj.zhonguo4118.cn

Py:   ", ".join(map(str, arr))
来源：https://ew.zhonguo4118.cn

PHP:  implode(", ", $arr);
来源：https://mw.zhonguo7118.cn

JS:   arr.join(", ")
来源：https://tp.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://uf.zhonguo5118.cn

Java: String.join(", ", list)
来源：https://rq.zhonguo3118.cn

Go:   strings.Join(strs, ", ")
来源：https://ee.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://bz.zhonguo4118.cn

C#:   string.Join(", ", list)
来源：https://qo.zhonguo7118.cn

================================================================================
来源：https://ee.zhonguo1118.cn

E. 字符串处理
来源：https://fi.zhonguo3118.cn

================================================================================
来源：https://ku.zhonguo3118.cn

[E01] 拼接字符串
来源：https://ej.zhonguo5118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://er.zhonguo2118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://dy.zhonguo3118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://qo.zhonguo3118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://wp.zhonguo2118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://aa.zhonguo8118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://tt.zhonguo2118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://sa.zhonguo5118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://gc.zhonguo3118.cn

[E02] 重复字符串
来源：https://js.zhonguo2118.cn

Py:   "ab" * 3
来源：https://wi.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://fu.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://kk.zhonguo7118.cn

TS:   "ab".repeat(3)
来源：https://ct.zhonguo4118.cn

Java: "ab".repeat(3)
来源：https://bt.zhonguo8118.cn

Go:   strings.Repeat("ab", 3)
来源：https://oy.zhonguo8118.cn

Ruby: "ab" * 3
来源：https://kh.zhonguo4118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://gw.zhonguo6118.cn

[E03] 截取子串
来源：https://ey.zhonguo7118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://um.zhonguo1118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://ac.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ru.zhonguo6118.cn

TS:   s.slice(1, 4)
来源：https://qu.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://qy.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ho.zhonguo4118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://zu.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://fa.zhonguo7118.cn

[E04] 查找子串位置
来源：https://fn.zhonguo3118.cn

Py:   s.find("x");  s.index("x")
来源：https://zi.zhonguo1118.cn

PHP:  strpos($s, "x");
来源：https://ko.zhonguo5118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://ev.zhonguo3118.cn

TS:   s.indexOf("x")
来源：https://wo.zhonguo8118.cn

Java: s.indexOf("x")
来源：https://rg.zhonguo2118.cn

Go:   strings.Index(s, "x")
来源：https://iz.zhonguo2118.cn

Ruby: s.index("x")
来源：https://cb.zhonguo4118.cn

C#:   s.IndexOf("x")
来源：https://up.zhonguo6118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://cs.zhonguo2118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://by.zhonguo3118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://lq.zhonguo2118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://tx.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://ol.zhonguo4118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://em.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://pf.zhonguo3118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://jx.zhonguo8118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://cy.zhonguo3118.cn

[E06] 替换子串
来源：https://pc.zhonguo7118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://fa.zhonguo6118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ex.zhonguo5118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://el.zhonguo6118.cn

TS:   s.replaceAll("a", "b")
来源：https://du.zhonguo4118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://my.zhonguo1118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ot.zhonguo2118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://ea.zhonguo7118.cn


<!-- 参考信息 -->