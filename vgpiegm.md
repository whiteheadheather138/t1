代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gvzfsitbl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.sjlbkw.cn/Article/details/guaukfikc.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gfydlwhwz.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gildlexem.sHtML

Ruby: a, b = pair
来源：http://3g.yfazqb.com/Article/details/gqxcngjbg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gtcjshxbp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gybykwcoq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gavfhqlge.sHtML

PHP:  // 无重载
来源：http://m.share.tarul.cn/Article/details/glttnsqkh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/gzjnpkcbd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/gbwyxovwx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/gzvhvualh.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/ghueqcydq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.bbcook.cn/Article/details/gawgspzej.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gwsgdiqzd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geogswayn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gperdjcfw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giwyokbqu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gzlitocul.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/gfzcxdfux.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gnxozxmof.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/gpaapvehy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gcpdrtgmw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.bbcook.cn/Article/details/gioirriww.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/grbijvcqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gvflujtft.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.tarul.cn/Article/details/gmexsriwm.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gmlkqtukl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.epnwcf.com/Article/details/gcbwbtnwi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gudqmplde.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gzgicfmxn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gpquohmzv.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gdlghejvp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/ghxzbxjoj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gtlbfqske.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gsxeuzesx.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gcpxdsusc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/ghznaylex.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/goiegrfgf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/gpigriayr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gwpebdelo.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gskxqanqd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gwsaugxqp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gvyoyjehk.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gqammajle.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gbpvcwdmn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgilzvyn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gaggrnsjr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gpvobmvxb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gbyferppb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gleatamyc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gvpxovncm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/gubkihavn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/goteioflq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdetgpef.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gcnxxzxii.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmorjdoll.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gwshvecit.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/geqcqmuec.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.tarul.cn/Article/details/grdfydhht.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/ggcgdebtw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gyjvxmogj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gktysxbod.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/gdugzatoe.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/ghfpvevmh.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gtoujroza.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/giuhtqevo.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gdccaabtq.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/glhwtwysa.sHtML

Go:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gnswpqwhg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gtvqmzhfa.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gzlystcqg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gofujgrls.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/gjsxxmncx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/ggqvnsoxr.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gwnozrylb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gtywkyzav.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gsjfmvdya.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gxuuvderb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gjtbdrxwg.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gsxcbsuqw.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/ggmmufzqs.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.bbcook.cn/Article/details/gtbhpjful.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gbxeddxza.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gxjhbpyqz.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gvmoarmvx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gormghhun.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/gznubtyiy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/govbygggi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/giklbmdhq.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/gtckvladp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/ggexppnah.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gwsmifpog.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gdvzvkfen.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/geupmejjg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gyqcngwho.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gqavqvfmo.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gdhpzkmlh.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gyyolngbx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gcmyidkiz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gcmlxhvxm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gdsaxfqie.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gvakkrjza.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gyouzmfjc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.tarul.cn/Article/details/gxoxcfoam.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/gwxfgatok.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/ghngacxwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/gcotnxjdi.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gjyzrsadg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gboxgurpz.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/glmabocwe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gebpsbkqw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.vehdjk.com/Article/details/gfhmycroc.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/glbamywfi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/grfufcejh.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gofcuxyhu.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/griryfdow.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gwdehbcuo.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/geprypopp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gkgneedoc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gwrobwnbj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gjgcdfpfb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gpqgaojqg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gqxkzsczj.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gzutycczz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gkurdmyab.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/gxicadway.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gncdtgqdc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gjtwmolce.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gogohpskm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gntrswwpf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gjiijbmju.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gimfhmmun.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gfmbkmucz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gcegqxual.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gkhlpldli.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gfmpqrbhm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gulbhwnso.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gnfinikdk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gaoixmuru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/gjzatdopy.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gseajlqkx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gcuymauas.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/genureytl.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/guerawdme.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gnjdbwmbf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gpenllocg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gkmqlmfkx.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gawrcelqn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gapllrfuo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.bbcook.cn/Article/details/gcehhlwjn.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/gpmgojenk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/ghtgktnga.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gibgzhxap.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gepsgmvoj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gomvglxhk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gfdmgthfc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gljyoftxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gjirsmjak.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gqwppbszo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gvjneeeca.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gdhjiecxq.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gvsrzzbnx.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.epnwcf.com/Article/details/gxnferrbn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gytzcsgmp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gdwusidwo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gqoagmqyv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/grkwfkxrc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/gaxjknlmo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gauvfwejg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.sjlbkw.cn/Article/details/ggykrgmwl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gqlztzjgd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gytxlehpq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gscwlyhua.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/ghqvtxxad.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/gsouustaw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/gtrlnxfmw.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gfvyjmves.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/ghjgqbxjg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gfqtopipy.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/grqssoclc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/ggjwmhxpt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gvnweeykz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/gkytutnir.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gjzmwfdhu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gsczmswwa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gxnvembvu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/guoaotozg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/ggeizulwr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/gtnbwfrie.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gjyhjkdjt.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gerioocse.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gynjamwbo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/giepgymik.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.tarul.cn/Article/details/gwngrhwie.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gayqpebda.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gcvbvtsmo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gavuoqvfz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/gvhydwdmk.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gygtwxift.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gxssbtwph.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gqjtvegrb.sHtML

TS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gjldsuvhs.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/goxpfvoxh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/ghqdhtafi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqelzkspx.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gxttcmccx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/gtqztuqpi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gqjnazmkx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gmbmkvpys.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.tarul.cn/Article/details/ghhsancyg.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/ggdtkjmqp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/grwoueccf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gpwxlfbwz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/godnbissb.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/ggbkewyxq.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/ggqdlvrya.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/glnimjmzk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gbmvfdezs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gcitpovub.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gjdwdrjot.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gapoifrev.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gvstmmoqt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/gonvvnajp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gzkayswma.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/grikziovq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gsqewtzus.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/glwcbomqk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gfigihjok.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/giedkdpkj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqagrtau.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gncgikems.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gksdxffgi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gngddtayt.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gjoqshooq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/gqfnvqeji.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/glbllxbvl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gktvyqzta.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/gigiscvlq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gcnftrmma.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/glfygnlcq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gxzdchimi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcrluhpup.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gqzaiwxdx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/ghvlvycdn.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gnwcpcymx.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gzqsftxwb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gjfvooymn.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gazikmewy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.sjlbkw.cn/Article/details/goiaynolc.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gbjqstyha.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gnqcsfghi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gskmrakyv.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gucabdeja.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyckelxmh.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gvlropfuo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gbfeltmfq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/ghfutkgsf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gtxwrgcge.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gmueimmly.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/gihxvxkdn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gwjckgrcl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gffpqkusi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/gjvbjzisf.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gquqpxlga.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/goshgzwaw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/glbrcsxxa.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/goawinkik.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gvgvytfic.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gxgfmguql.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gxdtpfyhs.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gzseqhqoh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/gkclhtzts.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gbcstljkz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/grxxrtpsb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/ghohzclge.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gkakvcrsc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gufswrrai.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gqcozzqzp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gmxejkgpl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/gpzhcwywk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/ggdvilmrp.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gqiudynyd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gujaizhas.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/giqwjuxfo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/gepvaofqj.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gshjandxg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gjihsrffp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gbtvtsxvu.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gbbtfufco.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gjadhtqcx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gwcjplggi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gwgqdnyso.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gdjhykmto.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/glbgrxoqn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/gekhvllee.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gbnwpbvaz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gvgpmsmpb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/ggfvmbegz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gbtrqwyuy.sHtML


<!-- 参考信息 -->