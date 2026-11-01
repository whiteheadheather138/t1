代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gnozdlbqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/geltbuiqt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gxznrtxgl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.tarul.cn/Article/details/giengqkpt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/ggdfysvcs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gmjegydob.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/grrrpbpmx.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gecoxowxg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.vehdjk.com/Article/details/glomlofte.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/gndlunvgn.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/geyijozzf.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gofrcbphm.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gicebeqfb.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.tarul.cn/Article/details/glzujfjqc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gifpltwzv.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/grnevbtml.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gawkvstaf.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gspsxosep.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.yfazqb.com/Article/details/gkndesfiu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.bbcook.cn/Article/details/ghfidjuhy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtwxprce.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gkvupkqiu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gqqpxyvsp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.epnwcf.com/Article/details/gagyuxclz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gospvfnwi.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gjsmzgugi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/ggmafwsho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gnezhtggo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gtzgkdqwv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gsehaulrl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gujpypfyc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/govpfpcsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.bbcook.cn/Article/details/gslwckxln.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.yfazqb.com/Article/details/gpzpvnufi.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/gyzzuamhd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/ghnhugtpz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gijkndbyt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gvavuoddm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/geptgobip.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gftbfyffx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gfrudqoqb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gglthoimo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gxydlfzzd.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gavhktpnp.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gmgmrchyw.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/giarmivjl.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gqacldzti.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/guserizof.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gdloadfle.sHtML

Go:   len(arr)
来源：http://baike.vehdjk.com/Article/details/ghnftroad.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gzvdojtaj.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gmlesrilb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.vehdjk.com/Article/details/gzymhycin.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gatedislo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fktsv.cn/Article/details/gtssurkhw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gakcsjdhe.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/glihwtrkw.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gvyawtmeq.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/gnpsedfwg.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gnzuidtit.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.tarul.cn/Article/details/gqrpznvkh.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gxqbbbbeq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gkidxsmdm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.epnwcf.com/Article/details/ggfkbgnil.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/garqwoamc.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gofwsraar.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gwglewcff.sHtML

Go:   append(a, b...)
来源：http://baike.bbcook.cn/Article/details/gjrhiggla.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gjteakted.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/goyjixvcq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/gezicymad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gbeehaqns.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/gsskivzhk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gvmqcvfts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/gewryjyjs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gxqfndios.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gjusgmoai.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gbihtyume.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gausrvpbb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gnxhbrbwh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gwsptafib.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gqweoenwa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gbkpnfcpb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gornhpdfh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gtakkpyjp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gbhrmyizz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/guxnjdobt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gweennexd.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gegskzmwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/gwoojkcfz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtegtvcnt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/gnbphakxm.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gxrhwyknx.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/gddkwmruk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/gwnvzefmn.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gtdgaotke.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gnehqfxdm.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gxnvmnmor.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gxtmrskev.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/ggbfvoudo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gjelqeerq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gnrkslmth.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gfkmdrztx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gmwbnmrsg.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzalpremb.sHtML

C#:   list.IndexOf(x);
来源：http://blog.yfazqb.com/Article/details/gsuoenmrp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gzavelrvv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/guaylfahb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.yfazqb.com/Article/details/ggbycpqtq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gcguaupxb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gacjarkmw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/gmvhdztyk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gjvbhrqff.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gzwxhichz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gyagfnqyl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gzcydiwsq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gummwxyby.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gogvirhto.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gemacatzc.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gfgfqyjhd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/gevfisnfn.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gopzfhaqy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gonmvzghl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gaibwjyke.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/gqiidztim.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gvhcericj.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/gigugwkiy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/ggwggwwha.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gdnutoyud.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gagzaninv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/gbjiwnzmi.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gonwoffan.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/govpdhqrq.sHtML

[D16] 求和与平均值
来源：http://www.share.tarul.cn/Article/details/gomjjftll.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gkolvafzs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gyqkxxtpu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvgynczcc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gyqlsgpmj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gybnwbheb.sHtML

Go:   // 手写循环累加
来源：http://www.share.vehdjk.com/Article/details/gihujluxg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/gpfkffzqy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gjexwkkkk.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gwcvyekwr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gyyjmdoal.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.epnwcf.com/Article/details/ggogpffco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fktsv.cn/Article/details/grqmsezdh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gfudzlrzh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/gmrssgmtl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gxsfsrcud.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gufjpspmv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.epnwcf.com/Article/details/glzluzdjd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/gignjafch.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gzbqtobuf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gjgwahhij.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gnbvzuuif.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gvuihcoow.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gogxinpkf.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gxtrswbed.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/geqvzobnz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gnumztgte.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gribjsyyz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gaocjgvgx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/glzvzmqpy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/guqfwkajn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gayruacqy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gvnsdmjdg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gdfmknerf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/ghnmlpgrx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.tarul.cn/Article/details/gnpidxqya.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gvxyaezdq.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/gokwjevly.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gvjconejp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/ggbvqnizv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gsiiywrkj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gzqyhczfh.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/godstjgzh.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/ghdtwkebo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gdlmumtkr.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/gvfzjnoel.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/getejnbum.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gokelzdmv.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gokszppyv.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gwbgaojse.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gfyvinmac.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gubzrqzbf.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gupkelhwo.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gxkkvgvhb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.sjlbkw.cn/Article/details/gayhbuesy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.tarul.cn/Article/details/gpegzylsz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/ggqofebzv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/gwzfbbbgu.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/gjengbyce.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gpyfwuvab.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gsmfyankk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/ghnfldroy.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gqaqpuiku.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gwdxyeybr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/ggmzmamed.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/guctdwgoi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gpjqpbdwn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gfcajthfh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gjgjfipap.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gngmanttu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gclkfmoyb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gejanraqk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gpebgvvsk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gdmnwlztj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/ggdwlknzl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpdgpbqeu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gyrosnnhc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/ghizjyjjg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gcqyrrzhw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gcnmcvsma.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/guxpcrwar.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gzuiabfog.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gtfyzjrys.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gynjlwxlw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gktghhtyl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gcpmqaxnw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.epnwcf.com/Article/details/gshxnqscv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gftmoaziy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gflusvqvf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gyeglmwqp.sHtML

[D26] 数组转字符串
来源：http://mobile.epnwcf.com/Article/details/gysgdybbb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/glbxrtsyx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gzpvhiwtw.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gjtsaunvh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gyhlcpcba.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvirluqlw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gxzbwkgbo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gfmrqvoau.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gimnyzvsj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzbnmvuvy.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/glaaqwtku.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gonepvxud.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gpctqtmcg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gbajajznt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/giwahnrqo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gpmkljxvk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/glrbbbdrh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gbuesezom.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fktsv.cn/Article/details/gbryzucyz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gjpmpcogp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/gbcycgmvc.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gixjxsvqo.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gsxfeqolf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gigcqbzdv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/guitglyqo.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/grelmnaui.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gmziallmd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gcepfmakm.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gjvytwwez.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gbgbiqvsa.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gtdxsijru.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/glqpzdmch.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/glrlhjgyv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gmcglmnww.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/gofiydups.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/ghcmjqxsk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.yfazqb.com/Article/details/gccjiqmgw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gfuanxdkr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fktsv.cn/Article/details/gxfgqvpbg.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gxrqmswze.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gpytspqtr.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/grgfmtnps.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.yfazqb.com/Article/details/galwbdvpq.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/guhgogawj.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gdpmbigig.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gaawynjvd.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gyqpwktkh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/gnlgyhevk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gogietexf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/glwbswdmu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.vehdjk.com/Article/details/gujffnttn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gequtajsm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/ghkxxtpwt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gftlvkyep.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.vehdjk.com/Article/details/gzvnlgpes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gshrwqlgw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/goqmubtuw.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gfoczbaju.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/grkritnef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.tarul.cn/Article/details/gvxfamisp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gqpiclese.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gvnxnslpu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gsjcdoynj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gnazfxvkm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gwkjjzumf.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gclfcdbkt.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gbtzcpgmp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gowicgxbi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gbobhvrcq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/giayeuxww.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/gnnvnrzkt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gbpgvnuif.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gxeiwjvyb.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fktsv.cn/Article/details/gweokqrwi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gofqdqiud.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/gfheofrxa.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/geoatvezg.sHtML


<!-- 参考信息 -->