代发 wailian999

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gaafetdxn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/goachywgs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/gsdwxnxxb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.tarul.cn/Article/details/goojptaom.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gxqckmrcg.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gpiynfhed.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/ghkxxvbtn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.yfazqb.com/Article/details/gsnorixpq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gvctfrrsg.sHtML

[D04] 删除元素
来源：http://blog.sjlbkw.cn/Article/details/gxyplhwhf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gjmiefvii.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gxvfwiwru.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gwpsynhrw.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/gmsdknocw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gnapfchul.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/grmettlik.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gacvmhexr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gvnlmscnl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gpnuwmudi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gbatdpaav.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gmksbdtrk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gcldrohgc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/graoounvt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gnydmsgxh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gapbhclya.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gowyfqday.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/goopuxydl.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gxtqsokur.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gwjzqlakw.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gywzexlry.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gqiadnyxx.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gvxhcnknz.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gaxadskea.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gshcoqoyu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gbfmddtih.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gpfqpsaqw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fktsv.cn/Article/details/gkpevkmyb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/gjgegvrys.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gqfufncjk.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gansfhngo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gkfgbniro.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/glbngnbdx.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gmdlixhbp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gqsbyymtm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gxihdzftd.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gjcnpfgkn.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/ggniczcpd.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/goxyakqac.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gbnlijaou.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/gehgtybvl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gqgcoryia.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gypmumlci.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/ghkmrpkzp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlpxoamt.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/ghasdjqth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gvakpxxjd.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gsobnzsnd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gsykuyknh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/gcnifyixu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gyossccrp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/goqgasear.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/grfrvqdfd.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gdjmcpdsf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/guirteihf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.vehdjk.com/Article/details/gqcpbvtvp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gtksgamdc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gqthnelzg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gmopyddmh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/gsmfsftgf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/gvxahbyby.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/gysqecils.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/gfzykynay.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gwlcarvqu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gqzdysvlg.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/grjndbrdb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gbrfpmkpd.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gkfybavpw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/gobeopdlx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/gjjfppdto.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gudcmjbev.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gqknwfakg.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gqrwtidup.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/ggoegcyve.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvaawknbu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gdkmdspjc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gxnpzdukp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gxzhlahcc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gsxupdvms.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gubvufvsq.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gatydxvwx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gzcjojhcc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/glmxpwvvk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gqhkhfpsb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gxyezgdee.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/glwjyhwqf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gnqbymlcq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gtzidtllj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gbxhijgyf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gshoylmue.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/ghhgmdyrz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gxlteccxu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/gchjaxrnc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gezslwiby.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gzctjcwqt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.yfazqb.com/Article/details/gpeqhkwka.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gncsweqbx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gyymqspbh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/geifaudxf.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gdndvauzg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gqzczudoq.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gcdqsgkvn.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gaceabmor.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/giiomwniw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/giqokilyo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gasfyhmwn.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gretahlgf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fktsv.cn/Article/details/gudpbkcau.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/giegjbcys.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/gqmlddzku.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrdcggjw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gohvcwmhu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/ghichmpcc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gxjmxfmau.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/ghcfgxafw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gjugaohka.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.sjlbkw.cn/Article/details/garehlirm.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gbsoaypsv.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/gkhqomxuv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gwofxsihs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gugtsdleo.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gsjxjqlur.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/goqwmnoqv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/ghtpbeyvt.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gxxiwejjs.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gweeowbls.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gojlcmvhi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gjhwtzodm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/gjnrkgzjv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gzsypfylq.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gixbaztwm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glvkcgoei.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gijypmewj.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gmgfkywae.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gcccuzpeo.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/gztiqgulw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gwufcysfz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gdtifjlrn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gtaefaeta.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gjeqldahj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gtnzwwzey.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gruzkjuve.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/ghgcxbxrm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/ghpjaioop.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gurnrgteg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gfkujapvr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gdysqjcws.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/ggrxwcrdc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gjmxttkpt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gxstmnryj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/glirgpdnm.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/geauthjus.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gptpoihpm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fktsv.cn/Article/details/gauozvsmp.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/gnsjfyfyb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gpdprlamv.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gqshnpyxv.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gqqavlgos.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/gehbfwvqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grkogtwhl.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gpchkxyzu.sHtML

C#:   list.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gxkajhuak.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gullxbore.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gqxjaeall.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gavtxdywi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gxcjdznvd.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gsrjvwmqp.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gayfgklex.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gxabfypsd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gyfkxrdch.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gzwwtxzgi.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/geweheeer.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gcrzwcfyh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gjbggtgue.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gexjwyupj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gpetxvoqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/glykwaezm.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gyznrmxoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.vehdjk.com/Article/details/gmsuxjzgu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gofavsfvo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.tarul.cn/Article/details/gndommnqc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gdnlnurjc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gnekuglvq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.yfazqb.com/Article/details/glsyabxht.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gbetchdhw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gzehwxrlk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gmkdcroez.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gxxyxepwt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/guhcwxqck.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gxfgapmaf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.vehdjk.com/Article/details/geautqais.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gxcxfavrb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxbnnysmw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gtofazyjq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gjzvpdlmf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gugxbfhqk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/goswbeuwr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/graugebjt.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/gwbdhafyd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/gujzirydk.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gmrbgzntj.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gvzditnvw.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gaqvcwjhg.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gdwpzykjv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/gyousojvh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gvdhdxlcb.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gwasdgvjg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/geuftvaka.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gntkyqiqu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcrasbgam.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gbsywzell.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fktsv.cn/Article/details/gchfwzjgy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gktemcewz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gcudixxwl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gywevxfdn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gtuqztrut.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gzchkknrc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gnbctlqip.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gkddsdwib.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gtnwywjzq.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gujleqhbx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gpvyijkbf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gxyogzhgr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gvzrrjeyi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gccpiuhjq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/gksyopwno.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gpdupjuir.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/gwkagkfyn.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/ggovlprsq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gaesoiqvn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gmfchqlhe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gbxuvqwdd.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gbkxujgbn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gzcpneaod.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gxifrqedb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.yfazqb.com/Article/details/govuqiuxv.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/goekggzuz.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gwbhoyizy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gprgunorj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/gayqlenpb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/gfrtvqlew.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gtfrvejwk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gdasktmlt.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gkqtjlvsk.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gdxnbahvv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gcxsimrej.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gglujpwcc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/gfomqoxql.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gjqwusvqo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gwrmhpypj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gowmfiawi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ghuilrhzd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/gvdgcafkc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gliqmjewu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gaqpeuqei.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/garjzzrid.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gfmockdoc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fktsv.cn/Article/details/gicpfzpis.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gkfgxbwou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gheinceif.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gazxzbzdc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/ggvmgjgmn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gmqcabcty.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gjzfzyswg.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gbfkrgbjt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gaadkhxcr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gctkzywns.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gvnwamuaw.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/gjoffbwup.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gpoffgqkv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gtciswftm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gjomirghi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gruvkobaa.sHtML

[E08] 数组按分隔符合并
来源：http://3g.vehdjk.com/Article/details/ghtnmndmg.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/ghlflebgv.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/gdwcorwju.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gutmwcvna.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/ghfyasdyx.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gxioqbglq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gpepvdwwe.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gzziibifk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/glebvzkin.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/ghthdkscn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gqyhwrzir.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gehhvfbgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gxlrxwntu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/guuyguwbp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gkvzalqab.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gwvhruuej.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/ghbxroblm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gqrubvmmy.sHtML


<!-- 参考信息 -->