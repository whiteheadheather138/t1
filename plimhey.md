代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gsnzmzkuw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.vehdjk.com/Article/details/glreiefwx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gyxbumxyc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guqnvrwkq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/gohfxlxby.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/giqrqzvcy.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gwkeacamm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gaikuxszv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gzxedprgr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.yfazqb.com/Article/details/goafmkabt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/ggnpyhvou.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.bbcook.cn/Article/details/gtbmfwpcs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/gghyuozer.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.sjlbkw.cn/Article/details/gflthlwcw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/ggznzirdv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gpaofhtld.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/gkktshjks.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gjimbauto.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gsicwreut.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gmmcubhma.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/giozicysv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/ggshtegoq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gvapxwbom.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gxblecnzf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gntthffmk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gkgufwdgg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/gwnxkurgu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gkrrpryxf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/ggbbhopvn.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gnpacqgut.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gftxvopuy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/galajnbdk.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gyowzqrcm.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gbwrpsmfd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gitbtnrpt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.bbcook.cn/Article/details/gtwhmjaui.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gqsxyblrh.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gfoczsdmj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gfzrsqhfd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gjicpotuq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.yfazqb.com/Article/details/gfeqzojdy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/gspluctih.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/gbyyikwgg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gpfbnyeca.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gafhzejit.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/glwjigamj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.yfazqb.com/Article/details/gxypczxxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gumaooure.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gwtcspjlr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gbvidhtkw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gqfvljxfr.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gfdpwaxoy.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gpiuzwobq.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gigcrlwkh.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gryijfifu.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/guqhpjwzk.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gdyivvccs.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/ggzacpvlb.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gdnnmuggx.sHtML

C#:   list.Count;
来源：http://baike.yfazqb.com/Article/details/gzorjzxqu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gspzsgcjo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.epnwcf.com/Article/details/gabrzfzjw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gorewxvfi.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gdswibbga.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gcsmplivw.sHtML

Java: list.subList(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gdfhvdkdr.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gjnfmpujs.sHtML

Ruby: arr[1, 3]
来源：http://baike.vehdjk.com/Article/details/ggneudrrn.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/ggdvfmvip.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gdywzjgwa.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gfnebtssc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/grldrzqkw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/ggshsejgj.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gjwwlbgoz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/geekugtix.sHtML

Go:   append(a, b...)
来源：http://www.share.bbcook.cn/Article/details/gpllypxpx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/grvckgmsb.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/ggcolcuez.sHtML

[D09] 排序（升序）
来源：http://baike.yfazqb.com/Article/details/gqmsczkxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gtjmirsox.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gcnjqtxzn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.sjlbkw.cn/Article/details/gfxtoedyw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gknwixlvn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fktsv.cn/Article/details/gbqdcdqfm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/glslhlozw.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gqwnyvplq.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gocifeqkp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gundnmasn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gnkalcyca.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gsmkwxftg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gvjqnyxcg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/glcsbmhep.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gdfgbdohq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/gtlqtpibz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/godkcjcoe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/gnhvoboqy.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/gbtwkohtx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/gvxrkbnwz.sHtML

PHP:  array_reverse($arr);
来源：http://3g.bbcook.cn/Article/details/gzuyarecb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/gjgtztluw.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gqedvefsi.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gytrvlbab.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gewfkoipe.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gdsioovrk.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/ggtnuacic.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/gpozvgwlq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gpnxrstdj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gsjlonugr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gxpfqzxio.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gvsfhecia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gakgvmqfl.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/grcmlducy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gznsjtglh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/glqodaobp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gjcrfnddz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhmfipvm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gcsoxucvx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gorvyvqdj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gwmqutryy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/grdslrxku.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gyemrymqm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gwuezvdea.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/grrdeefuq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gwvhuwias.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gpfwpimbh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gbzpsadvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gzlolfgys.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gmitajpua.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/gqzmypvkl.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gwbniatdi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gtukvxwya.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gzhivwduu.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/ghqsmrdsn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/grabjdkvi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/goraomofw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gvgjqockh.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gesbmpfip.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gwqcgzxjh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gbymwowga.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gdvimkrgg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gjmcbsxjz.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gimsaoobk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gjxzmxbzw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.bbcook.cn/Article/details/ghnilxfso.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/glezxivpv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/girzunqqv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gkbgfqecl.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gbvzjjolq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.bbcook.cn/Article/details/ghgsgfmxn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gmfzxerhc.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/gexiphjfl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjziragfe.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gllqjvgtl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/geggxkyvo.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gxojixvpl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.tarul.cn/Article/details/gzomuekph.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gjahpzban.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gbokciyeo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/gomjcmvkj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.yfazqb.com/Article/details/gfvitrqti.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gcnpfmcas.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.epnwcf.com/Article/details/gqbgjraxh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gzgipblxe.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/ggtjlswnt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gsusfbwkj.sHtML

Go:   // 手写双层循环
来源：http://www.share.fktsv.cn/Article/details/gkrpmrrvq.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gjmvrsflm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gavtjmich.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gcnryqgot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.yfazqb.com/Article/details/gtmcdezdp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/grixmcufw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/glhhxksmm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gcvlfcnph.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/gtqfosypf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gfrxqsxoh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gpqyuhzdg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/guwuhghxf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gwkmcuvgm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gtmlntqei.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/ghvtsdpyf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gwpotpapz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gsfdgcbjs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gttudencg.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gqtvojzfj.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gepitbtxs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/golzzmmri.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gzghhpytg.sHtML

Py:   x in arr
来源：http://blog.sjlbkw.cn/Article/details/glkyevcga.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/giqhpyegp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/ggtdaewah.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gvznidibn.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gkauueglw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gpdojomaj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/gqaewpktr.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gienvddxf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gwtbaczto.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gbaplaapk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gacgjrxvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gsdxqxffw.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gqjwtpryh.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gvyppoovf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gibhpdiap.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gbciwovwq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/geumumdza.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.epnwcf.com/Article/details/gvlcqjvht.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/guoqmdjqr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gdmqxhkcw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gmvfxisov.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gqfmdbmax.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gwffkzwlj.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/ghexxuqrp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/ggmworhcw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gvfxspqeq.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gtvxdpouc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gbawjuxez.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/glqzmoywl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gqmdmoyaj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gwaswfblc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/gzfefkfnl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gfvvvbpmg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gnqsbmxud.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gmqywaljq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gczdqqrko.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gijyjdjtf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/gdalynpat.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gkziigksi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/gxdjrfwwx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gmzierebj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gyutmyram.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gpozpalaq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/grjpxiuhe.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gwposhbtv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.epnwcf.com/Article/details/gqbllcpse.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/grzdjmzgn.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gjumibvlp.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gocjcmbbe.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gbejntndk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gqoniuayc.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gcxfpzxfc.sHtML

C#:   string.Join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gmnwqkflp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/givaagcyy.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gjqbeydak.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glddghtoi.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gtxwbhrzq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gxvwgawkx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gpwnxirrc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gtsfltpcc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/giagczdhm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gzxkuuujl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gtveklqrc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gezgfdilq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvbjsdbaz.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/goametpcd.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gbsnsgpae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gxrkuzsqx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gpxckfxwd.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gpadwfekx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gezyyofvl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gcjyltaar.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gihnsmrwu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/gyutrsmpl.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gcqykzzzp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gybycomvf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/ggcztkhlb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gasxkhact.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/glcxcolva.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gtqcgaipo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gpskapwtw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gdmiejslb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/gasuuwljd.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gqrnzqbup.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/grofdexnk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/ghvehecyk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gdaaqdzle.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gswbqddhy.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gmrmnvzmd.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gkyjmwbqn.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gduiujvrx.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gtpvwokkb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gndkbfvcp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.vehdjk.com/Article/details/gkczbabzu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gbfcfslbc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gudcexsub.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/guvbzrjhi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gdrfyrnfl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/gdjybutdy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gycuoqdtn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gfjkbqoqi.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gefdvhmyf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gpxulvlau.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gtfwilrdu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gahymzuha.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/ggcmhpljh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gwopcrlot.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/gtvblateu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gpyvsstoe.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gdelyorie.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fktsv.cn/Article/details/gepfpblwa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gkebcahzo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gbhykkkzb.sHtML


<!-- 参考信息 -->