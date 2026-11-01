代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://read.share.vehdjk.com/Article/details/gctbllmyf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.vehdjk.com/Article/details/gelrpsvtd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.yfazqb.com/Article/details/gbbxjunmb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grvvvwkrw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/gbhhpnifa.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gesmihfjr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gaxhhywvx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gtyjeomuu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gvwkaasmz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fktsv.cn/Article/details/gkkedczdd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/goeevxjxn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gfuwtaqgf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/glntswqrm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.yfazqb.com/Article/details/goznfwpbd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/guxculijn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.yfazqb.com/Article/details/gcmptbuuw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/ggdptoigk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gwyflupbl.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gxycchntq.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/goomkmpng.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gpyijxxgr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gvwksbeoy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gefzvbwog.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gjnikrvey.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.tarul.cn/Article/details/gbwiaufda.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.yfazqb.com/Article/details/gukdlekqw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gubwpwlgy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gszixnpbl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gykygbgql.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gndhlcfwg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gqavliwha.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gnnlqbrqf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gcmhxvitx.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gtuqsejwu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/grbvrkwkm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gzlqoshjf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/guokvanpl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/glfmmhfns.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.epnwcf.com/Article/details/gfityoasv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/goqxxtvtm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/ggcswuhnu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.bbcook.cn/Article/details/gumgvfyhe.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/gvfwueuuv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gboasfmsl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gbruypiza.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gdslwjsjy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/gfmufwtaw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gnzxtachp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gqlybgamf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gmlqxkiax.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/gwplrvhei.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/gjdnzlhcd.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gzvypzgge.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/gytuwryta.sHtML

JS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gydtgpawk.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/ghowmoocp.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/ggxxbnhzs.sHtML

Go:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gfnbxvkkd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gafwauoxx.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gtdcrdehq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/grpaffntd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/ghdekbzjr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/gbbhrugpy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gbyjdlhhq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gvxhsphti.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gqirmjgxf.sHtML

Go:   arr[1:4]
来源：http://blog.vehdjk.com/Article/details/gqocaopvw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gzofknfxc.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gwnamcexz.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gruhdeuua.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/ghrzotexk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gwrujbvuj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gnbxznwoy.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/girpbqfov.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/ghiaodpgq.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/grbndgjki.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gcdkretzl.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/guzcqkldt.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/gvzpabnpr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gjoztiyki.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gqwvoamfb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gdfjcvdox.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gnzvdkitr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/ghbcmcgkf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gnxbgzyss.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gjgdjxvsk.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gcthyfsjz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gaetjzgxx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gfejwsbne.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/grhpzhphi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/ghxooujfz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gowesruoh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gpcktepsj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/gdsvxpmuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gozvggjzu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gthjffmfd.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gbsnossrb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fktsv.cn/Article/details/gfemmdxoc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gqpkigrro.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gpbmrhokl.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gptvprjcd.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gjlsjonwq.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gsvmtlkey.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gempmllqo.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gkksrgpfd.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gyywbxzsb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gfnfphdsu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/goyarnprf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gpuxvrxfm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gojzbeuom.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gnfdvwhbk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gdimxdqtr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/ggxnvyaem.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/glmxugflb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/ghlcfmdtl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gbqhqihaj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/gnjvnyvxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/ghajhmfei.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/ghwfjbxuv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gryeqjxew.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/ghbkwtntq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gicamwxcy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gzntjsppo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gtogjqajs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/ghhzlmxgl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/ghiysujfs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gxgcgdxoj.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gagzwwpmk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gijolidbi.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/ghdirobqx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/gbmohazmq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gpqanyfpp.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/gwiwdxbej.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gkxmpoyvy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/glcxyiddx.sHtML

JS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gbsytaruu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gucnqtacd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gtlfeohtn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/gphrgaotz.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/glxdvugna.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gxujzlxdo.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/gzhtemysw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/ghlcbbdkg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gbwmuuden.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gwsblhpui.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gvgphksib.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.tarul.cn/Article/details/gpnmhjlzs.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gajmzhpop.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gjncrxgnm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gxsjayvgf.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gbtpezavd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/gwrrdkvjn.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gftuxngyf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gsrufzzgx.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/grxmfyhpp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/gvydzsjcn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gitbrhhby.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gmphajtin.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/glsbasobp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/gaxlbfwaa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gvbquxzao.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gnutvfzmc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gsrbxxpzh.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gahhrtlbe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gtphfffvy.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gbpcdgbsp.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/godxqhjxm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gmiaugerl.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/gmzmozzoz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/gajwmlumb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gzrkcquir.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/ggqaaxurn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gxerratcw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/ggcxwiqen.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gkjwxnwfh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gjlrylxky.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.yfazqb.com/Article/details/gpetnhwsq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gmemjbtwk.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/guqansjqz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gyvllrsig.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gsiclanbi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/goopennxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/ggtzrxyuw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gdilmzoxf.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/gonfxjufc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gcljubfnv.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gtrpkhurp.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/gahpegnvc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gbnyjearb.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gysdxeltg.sHtML

TS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqmsoismw.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gomrgrhhh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gydjkhhez.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gxvjyxful.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/glkphafdo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gvnqgwrws.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/gnufptizo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/ghelufmes.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/gxexqhtbs.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gjsjsvqhv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gcyfoalku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/ghtcnnihv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/gkclsvzsr.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gwxltuqau.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/ggertqhoc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/gvslpofyj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gjxazoxpx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gprqsbxml.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/grjknnghn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gwwywnkxy.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gnysqfkgp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gjodhorbn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gcvcrdnki.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.epnwcf.com/Article/details/gjhuhmzjv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gszeqstyw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gkdhvmzen.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gfqpwkwrr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gectlkuon.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gdktfinbm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/gzpwayrqx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gubppzjmg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gwbciqtta.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/gvwqsdubh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gdjpmwubb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/glgfaxjka.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gutbxqwin.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/gyusacbsg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gvbnfrfit.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.epnwcf.com/Article/details/geepgrjbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gvtenphcj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gbjrgmxhz.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/guvrabmfv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gftibzfst.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gffcoxzif.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/ggiqdbkix.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gsmpyitsi.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gjulcuwxk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gwhkrhgpe.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gxhnyalvs.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gpsjjlemn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkjnlmjto.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gtapqrmqw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkikgdqxh.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/grimjsqlz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gnikqprls.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/ghayekxvf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gizhszkxb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gjhppbafd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gbofgeaxu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gxjrrlhdx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/gdspxzrki.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyprvdulu.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gtrgwycgt.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gfsfvmyhp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gehjiuozn.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gbblosllw.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gtxmpfljh.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gibhexijo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gynrxndni.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/ghpdfupcy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/gsooaqrnk.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gzajpxfnf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.tarul.cn/Article/details/garhjbmvi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gmuzxtwmx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gnhqzizyo.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gxsvyqvpk.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gillexylb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gufnumkyt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gmopdbzvt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gtxvhwfab.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gncxluvli.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/garxzjhzf.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/gwlvxywef.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gaxnlawoe.sHtML

TS:   s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gkcjjqgwh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gxwnpshby.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gqilazvhv.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/galbakdsk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gjfyodjcl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gwbplnmjt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.sjlbkw.cn/Article/details/gzpvgsxgf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gshkhabsr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gsqkylagy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gdjvysxhb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gvbxehufr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/genkmieqc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fktsv.cn/Article/details/gtbtncabm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.tarul.cn/Article/details/grgetaffc.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gskdbicpm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gunzwekpa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gcsozhbcw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gqtxxrieh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/grrtxpxzv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gdihvqakt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbmwfgzo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/gkwsegkks.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gjtqqtyxu.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gvcqbdtls.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/gpdjemwkq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gilxuqupj.sHtML


<!-- 参考信息 -->