代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gtowidsgk.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/gslzltcod.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/guprlbciy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gvvqsxakf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gvqtksmmv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/gdqymyjry.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gjdhdjfpc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/grdmbqdvj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gcqlqjllv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gfmboyvbk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gdfbplvrq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/guuwcjhqo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gfwvbbzur.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gclemxepw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/glgoqircj.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gzyitxccj.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gmhfwyuqp.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbivbjpo.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gtivrzxxl.sHtML

TS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqokatvw.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gieysqcxy.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gwdnidkav.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/ggftedbxa.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/ggoppxcmt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbyuqnm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gxdkxmysw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gmymsaiqc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gjdfyzdza.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gnatfpmju.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gfgecnbtv.sHtML

Go:   arr[1:4]
来源：http://www.blog.epnwcf.com/Article/details/gtjcshooa.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gchxbbzkq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/grxbokkfd.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/grhrxuscc.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gyrbtiiol.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gsvddrpaj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.vehdjk.com/Article/details/ggwznboea.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gntpcbbqp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gugihexcb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gdhwljsic.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gqvslngyd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.bbcook.cn/Article/details/gkfylgfug.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gccfrhpib.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gdpsmeaxu.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gobqinjwd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gogbtwqvq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/guzvzlbzf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gfblnqxwy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gqawdpcey.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gjahwlnst.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gulvcgnqe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/gzoyenuqz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/glabuimrb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/goqzcfjhk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gjqqtrtwh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gxllfukxf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.vehdjk.com/Article/details/gnvcrfzyi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.vehdjk.com/Article/details/gtcovytkq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.epnwcf.com/Article/details/gtvczctgd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gmwenghqi.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/gccivyeji.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/godlvqsvg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.tarul.cn/Article/details/girnxqyyn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gvnjtgzom.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gbpyvimte.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.tarul.cn/Article/details/gpuomsciq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gijqvmpki.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gslwolagd.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/gbkxclqno.sHtML

[D12] 查找元素下标
来源：http://m.share.bbcook.cn/Article/details/gyclmycrj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gzjxppynm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gzuaxqwul.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gpbxjptff.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/ggysbowyh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/gzwhfikwk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/giokvchpe.sHtML

Ruby: arr.index(x)
来源：http://mobile.epnwcf.com/Article/details/gnqalhume.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gmlojtzwz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gkhobmndh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/ggiqqzfsp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.vehdjk.com/Article/details/gvtsxkgaa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gdvdfrxtx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/guxzloitz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gjajrvicy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.epnwcf.com/Article/details/grlntiwas.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/geosejdhb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gfiipehtj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/gpgwnpqrg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gtulfsszp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gbbcfkris.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gdqsjiama.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gdwtnqtzw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.vehdjk.com/Article/details/gtahapbtb.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/ggpaghyry.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gebspmidv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxalcxxuf.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/griojaxml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gplutspup.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnceizozk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gakfjqkob.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gwwbikqzl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gqsefnjbq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gmyrbnosg.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gfprdbbur.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/gkztxevkw.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gbinghnnm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gjsxmizys.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gqpwljevd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gdlgmdvcd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gjhjhzbwy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gutfisllc.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/glqnoxdbe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gqywiqdzv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gtqdccapn.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gcvmqknuh.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gboinzqwv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/glhwlrmuh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.yfazqb.com/Article/details/gjrdrebym.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gmctpmunb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gdutxhvsn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/gesqheigw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/goonriuzi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/gochetpkz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gsqxidjji.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gpawbjoal.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gyqnpofkd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gocskujss.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gqklmdzcl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fktsv.cn/Article/details/gjpawupqb.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gapfqkbpy.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/gyvuomiac.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gvddlnyny.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/gqilzrjcm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.yfazqb.com/Article/details/gemwbyolz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gtbflnfiz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.epnwcf.com/Article/details/ghbqbxjhf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gonlptgri.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gqqlharqu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gidaltqmk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gyibhyahh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.sjlbkw.cn/Article/details/gerxupjzr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gvpaiqwth.sHtML

Py:   Counter(arr)
来源：http://www.share.bbcook.cn/Article/details/gavdymxcj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/guiumwctg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gnzucosrs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gwvhbyqpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/gimljapiv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gvkbdcgxy.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/gffvdkygd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/gatxyexlp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/govmyxkev.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/giljkoevx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/gnizhvssd.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gjluncyig.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gzrqrffki.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/grmjwdxim.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.tarul.cn/Article/details/gfqlplbpn.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gtoujwtaw.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/giklmwxhn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/gygfxghmg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/gaezixize.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gnjbfmosv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/gqciahwqh.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gtzfkhyoo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gzerfptln.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gdxbfqnvj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gmckrbfjw.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gnxkcpcjc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gimpnbhnz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gwjtguakv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gsnzxovoi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/ggejkfbfd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gluhauexi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gblvvfeze.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gcwafxyui.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/gidyqiumb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/gjlwncifo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gyaoynemr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gpmulwpqr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.vehdjk.com/Article/details/ghfocdrck.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gcusmyroh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gubznykfp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/grvgbzryh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gboqkzcce.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.bbcook.cn/Article/details/gdeegparu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gblfucxkl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/grlnypkqk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/gwtxkzzny.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gbzjvewln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gpkxgrnjv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/glzdkcmwt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gelclptdl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gcethaoth.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gyimpblgj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/grrjrzvha.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/ghlzeobhx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gfhnsghom.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/gyptztomy.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gbjimeuaw.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gngrvcfxt.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gajgjcsim.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/ggjxmumzq.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gpfqpekis.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gpqxcuchk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqfcmmalv.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gzdtaspqg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnmrrudwj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gnikeqrnv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/glvamucmt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gbcjhzoqt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gcyqswebx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gbmczluch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gxqqnvtow.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gqobijbso.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsckkbbl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gcsvheyje.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/gewnejcyj.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gunjfyuhs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/gxdqovage.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gdyhndhmk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gwwtfqwnc.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gjkjimakg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gtoexhagc.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gcwaupdzp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gkjdmjbyz.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/gxgzdtbxi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gdtlinhvu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gkgmmwwei.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gdyxftytv.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/glsjwduok.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/glcztvjhg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gdbpxxijz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/grazalgia.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/gbzlnlche.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/ggewmyypi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gwdxlzscm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gesmnkzbx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gskwltgtn.sHtML

TS:   s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gzxxphioe.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gchiudftc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gvwbwrixm.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gvriqmdev.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gcbdlizof.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/guukhcwmb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/grwcuehxk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.vehdjk.com/Article/details/glsedsxfl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gkfnwldxp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gcvbzcurf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gvmdpvfdc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/gsmcnjeqa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gwoswvpte.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/grfhgqtig.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gcyakdbmr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gckwrhsoc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/grdzyglgq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpdtxpav.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/goludmaox.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gzgueouqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gmjtnrhgb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gtrywlvfh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gcialwxtk.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gxsdzkwdw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/ghsafxcil.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbalebddx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.epnwcf.com/Article/details/gengyfher.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gvslnurkh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gmktoksbt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/geybcywhx.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gnscdsrcv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gvkcdaekx.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gamexodnw.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gdxrwkkpt.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gvonyswps.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gfggwpcyz.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gopzwunmu.sHtML

Java: String.join(",", items)
来源：http://blog.epnwcf.com/Article/details/goaciqlyc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gstnyxsnl.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/grixmbwxv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/goneuapjj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gnuxiwmqk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gryyhuerx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gyhthwabn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/golbjypwj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gppcthnit.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gzxebzrve.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gwblqwmio.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/govafgcug.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gsaibhawi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gmajhexzd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gplquvdtc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gwqbaznel.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/goptbcmps.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gqpkbacxb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gawxsiyqg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/ghciamgak.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gjfrfhvxl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gttryvslp.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gwdzuktod.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gqglredft.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gduemynxe.sHtML


<!-- 参考信息 -->