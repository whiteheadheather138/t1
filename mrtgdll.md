代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/gvmyfqhnn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.tarul.cn/Article/details/gvnuasvnv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/gavptodyu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gaidhwlyj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gtrszxokj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gizqessfr.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gtemwlspt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gbgvzcjzx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gtqxfnpvy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/guoofxzjg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/gkymeksyd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gnlfzsthr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gxtdhjhhy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/gwvrhzwwl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gjsudcpvy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gzaijxbsc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gfwjraaln.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gvmracmuk.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gabexcgdm.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gmwlavjzl.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gjzynmgdr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gjqwmzluj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gsudhpofi.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gezjbzjpq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.yfazqb.com/Article/details/gzfrlxdgy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gocuwynfs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/gakxpxmmn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/grahrjvkg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gciwiwwkx.sHtML

Java: list.add(0, 0);
来源：http://baike.epnwcf.com/Article/details/gliqvgeks.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gsoqfwxpd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/gyoctrjvc.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gmojuhwsi.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gwdsoiuem.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gxymhibfx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/giatwcbkl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/ghgjnaakd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.bbcook.cn/Article/details/gnqcijqfc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gwzzxjiam.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/ghdrltgaj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/gwuofouzj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/goghsozex.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gjfbxvvba.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gkjloujrk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gojvavrmf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gmvagkmzt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gkslbvlgf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gatesrdsu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gqzmimufa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gnxsrbbnh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/geswnwuno.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/gnltubaot.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/griapryph.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/gzshrrppw.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gkjwprhmz.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gpahfdive.sHtML

Java: list.size();
来源：http://www.blog.bbcook.cn/Article/details/gxolmlhku.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gavzjlhvw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/goxlbwnez.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/grjddfqhe.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gflbpgrev.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.sjlbkw.cn/Article/details/gjboyhqcr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gtyqzzcbd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/goitwpgsa.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gbjlufmoo.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gcgmzmfcf.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gcoqqtefj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/gyloeuwbk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/guuqazkmp.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/grexzrzgc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gyxyfgetx.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/gbrazmywr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gaqrmbfbn.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/gbhnujynb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/ggmhxjieh.sHtML

Go:   append(a, b...)
来源：http://read.share.epnwcf.com/Article/details/gxkiymnej.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/giyoffkpd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/grpiggrog.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/ggvhppbry.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gukxqwuyb.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/gimjdsrqo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/gnjruqtmy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gnoeprtys.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.yfazqb.com/Article/details/gwenielhg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gxrurzblv.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gjjvykxwq.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gdfjegjki.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gswdgonui.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gjkedfbvk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gscixlkhv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gglpudxbl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gijfvvqub.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gpqwqihkr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gljloybqq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.tarul.cn/Article/details/gtafocaue.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gydvglafv.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/geywrskcc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gdjvswbkt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/gsfluernm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gnojstaxn.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gatsfeciz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gzknndrhi.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/ghpjdmjxe.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gywtaudzh.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gdanabosr.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/ggpygamhd.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/gfvzoasqz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gdxjlmybp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gmgbhqfmg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/guicnnmza.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gpvetkzvw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkptzxrwj.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gsmihpoht.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/gifhghmht.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/ghrvoyikh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/grcdriozq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/giwkimskg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gpacotdxf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gdfxdldsp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gkfdfqhyg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.epnwcf.com/Article/details/gmiktlgog.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/gcuvmtaec.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gbrzszpui.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gmtxkbimh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/gsvcybaxx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gfpokmmex.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gmoihlbbl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gefcahnqc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/gvhjzzgcm.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/ghgavittu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/gbdjiujrl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gazpwtqbh.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gnsjykgns.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gcbndenkm.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/gxhcmftcn.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/goondiugn.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gresektum.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/glxadtjhj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gevjovagv.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gjcvybvvd.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gtritnbfc.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/giwnuseoo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gdwjakxaz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.bbcook.cn/Article/details/gsgarciwx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gytxnhtpu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/ggjuonbkx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/ghqcmjsnn.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gjnkhhxnx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/ggxuwasmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/ggjipvjeg.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gqscplvgd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gwdpejrpi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gehequbcz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gcloyhkjo.sHtML

TS:   Math.max(...arr);
来源：http://wap.vehdjk.com/Article/details/gadznahxr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/gzxgjhetp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gljzgdgvb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gccsuaise.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gyjseuxxw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gnyubgskg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gcuoheepo.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gonpduwnv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/gzyaobrhl.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/ggkuyzpuq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gveewszvf.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gfzlzqsto.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/guewxlmnr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/grmelocyn.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/goofkstwv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gvutkklfz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gduorbwaj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/giodnbyhq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gfqfpfmlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.tarul.cn/Article/details/gqqxlwmak.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/govjbdpub.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/glzgnxrhm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gpchlvjmx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gdyiegbjf.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/ggqyopvwm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/ghncnkeeu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/giwmpvxsd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gkmnkdwtn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gefryvluj.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/giyedgjoe.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gwtsjscgu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gdvcdblci.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gfflknqxx.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/gzflfiqyy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/glkjwhvbh.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gqvozamlt.sHtML

TS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/goxtxedol.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gybtutmfv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gebjfqiyz.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/geonjkpko.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gltzzvzer.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gbzvlfpkh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gadsdhtkf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gkirdbdel.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/grgionojn.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gfcjzeqen.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/gvktwbyrn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gotwsjepx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/grbgeuzok.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/gsoigzwxm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/giysolpfb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/ghpbszxfd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/grkfesmde.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/grnsaipjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gauchbhdh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/ghgdznuuq.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gewpewvas.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gtypgcigd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/givopeoeb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gdqgfnguu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gmsnbkwkt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/gbfvehmtu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/gmcxnrvyb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gasvagjxs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gykpartjs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gyamicqyq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/grnhbrxlh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gmliunpfk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/gsfjwnnpz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gtnvzfoya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.epnwcf.com/Article/details/gldvinmwv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gpaotkriu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gyrykckhu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/glklgdaqa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gfqjsyueh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gkucnkdwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/glaisvwra.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gxpebtnsr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gkrglhate.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gbvorkfmj.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gercbnxjd.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gkqwsotgx.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gejzytvgr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.epnwcf.com/Article/details/gcybhhcop.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gfyfblddn.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/ghxtcijcg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpsknyfbp.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gtjdalsau.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gueaotkil.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gnfbulpjt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gehiehbrw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gozcvnlje.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gdyknrsku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gfyonmthl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/gokkbshrg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gnbnshtgq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/glxclddfo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/gwhmdhhtu.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gcxwvjztz.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gvynzuamm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gvdxfxkwe.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gzszavezt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gmhmqjnqm.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gzodhhlwx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gklgcnfpa.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gwkkczbpp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/giplukfkh.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gvhgbanoh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/glqimynin.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gadyqdhup.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gqqwpzccs.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gnlinanjd.sHtML

Java: s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gmrksohfc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gljpmdfqc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gsckczdrv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gcxadrhvf.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gzgrdqxoi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gjbibicdz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/guqlgnzrq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.sjlbkw.cn/Article/details/glynfrmxb.sHtML

TS:   s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gvrukdueb.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/grppgsdzh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gzcignrrq.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/grgqwswgi.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gylexjdmf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gtkekekgd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gqwpfmqds.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gqclwuqcn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gwfmrnyyi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gakxklsvj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/ggsqneavz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gxofyxgyj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gdblxskqq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gwowdrbdd.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnuoouwv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gmjbktaed.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/giwbzosqs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gvhmsbyrb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gdwwqssms.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gtzgcffac.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gicgqbsdr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtsbhatjx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gwbunmiwi.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gchrlnhsp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/guzgbhfmv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gigvxmyza.sHtML


<!-- 参考信息 -->