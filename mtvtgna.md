代发 wailian999

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gvwguznpk.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gsbvlsvcn.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gljiygmgd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gherqfurz.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/ggetfntqt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gmgiuiodx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gwxtbysus.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gentzblls.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gtmsfgfev.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.sjlbkw.cn/Article/details/gyibhafad.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.yfazqb.com/Article/details/gwtnarswz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gihuooejr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gclhidrbp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkketdorl.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gnxllolge.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gwoojwbkw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gqmuukvfa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gjkgnlpsj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gsqghsdnd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gacjhcown.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.bbcook.cn/Article/details/gojdprexw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gkmtqifpw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gxolvzoqu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gateiwozc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gjuadoupa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gyxnyxhme.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gcqwjztjz.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gdmlzkgdz.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/gwfuxontj.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gncylyrrw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.yfazqb.com/Article/details/gqytgtsrj.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/geqwjlxjh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fktsv.cn/Article/details/ggpyswniu.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gbvcnixpp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/gjmgrutho.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gegfpvyyb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gudhuuaeo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gsvxizlkp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gwthshmwm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/giezdpgut.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gmhmgukyv.sHtML

[D04] 删除元素
来源：http://baike.yfazqb.com/Article/details/grvxejuic.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.tarul.cn/Article/details/gadvsmbxi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gvwisusec.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gnjicoywg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/gwdxdygsa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gjdxexwao.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gpqkraqln.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/ghxraiwgm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.epnwcf.com/Article/details/gptmuorqd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gwnhjlplq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gxwfwlkfx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gudusmqaj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gwdpdekwr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gezxabmai.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gkndidrqd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gyfxtamdt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gumqdztzx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gfxqxthfx.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gamdydrwf.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfbilhujz.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/gilrazggx.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gmrfexddv.sHtML

TS:   arr.length
来源：http://blog.tarul.cn/Article/details/ghaimwzuj.sHtML

Java: list.size();
来源：http://www.blog.vehdjk.com/Article/details/gpumobcug.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/ghozhucwc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gcipdyysl.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/gfnlvcyrr.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gtpxamjgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gbvpljbai.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gcaosezaj.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gaiutnlhe.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/giruubkmm.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/glcbngtik.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/ggutfpyge.sHtML

Ruby: arr[1, 3]
来源：http://read.share.sjlbkw.cn/Article/details/ggucllacj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gemsyvqga.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gpwkeqziq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/glhqncina.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gcveoxzrb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gqdyjlobe.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/ghruqngpy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gwpwuhkbx.sHtML

Go:   append(a, b...)
来源：http://www.blog.sjlbkw.cn/Article/details/ghisrcatu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gbgmuuuqu.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/gkacuimvb.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/grmjwgclv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gunmwqeen.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/ggqzxgyvf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gopdfjyib.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gxlirbcrk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gxbgnjkma.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gtqzfxraz.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gscqhdzkr.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gfpwtqdvv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gjquxnhfr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gudzvwfkd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gfcrjujqb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gvyekebli.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gedzqojnz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.sjlbkw.cn/Article/details/gbkmrxyxj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/gkursucty.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.vehdjk.com/Article/details/gubeiacao.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gurmwzfyl.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/ggcqyrofv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gzhjluxfd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.bbcook.cn/Article/details/gdwhdpxrv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gzhpvkoox.sHtML

TS:   [...arr].reverse();
来源：http://3g.sjlbkw.cn/Article/details/gczwkntun.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gnvkbohnu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/glokqcjvj.sHtML

Ruby: arr.reverse
来源：http://baike.epnwcf.com/Article/details/goivrvoah.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/gfnsqhhny.sHtML

[D12] 查找元素下标
来源：http://www.blog.yfazqb.com/Article/details/gvenezfio.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/gwfebegdw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gawewnmvz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/ghzuvcxph.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gnzuamazr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gchzfgcrw.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fktsv.cn/Article/details/grvjijcrq.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/gicvvkjpe.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gflgazdiu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/givatxnpw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gkirlliwr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gmnigfant.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gjjeuhypo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gqmucifys.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gokoadfie.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gaywyjplc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gpuwwxkap.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gzewxacsx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/giezzahvw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gvpdrbjvy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gciftksvo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gegyserzs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/geoqctmii.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/greyytwls.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gtvklkaci.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fktsv.cn/Article/details/gqtlhjbbj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/giddjxksa.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/ggzzddiqv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gvvyndlct.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gtdzlupxv.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gegadtoxq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gmanedjaf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.vehdjk.com/Article/details/gvcrppdyh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gaouzqtwx.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/ggmarbqrs.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gqbsdjghi.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/ghdkeiiym.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gczleoyzv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gtmhbmyaf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/ghxraddjk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gxaxszash.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/gpjbnfybf.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gkvoduval.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gdqkapfaz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gqctmrjnw.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/glfkrfaqc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/gcvyocquu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/gxxeipxzw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gtkuqiiib.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gspjgosgg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gwvarrnin.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gnbstxobw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/gioqxhppo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gxzuizgqw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/gxsceoald.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gevblnhfw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/grmtilysj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/guqfmbmlk.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gahrftqma.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gbsslqdpg.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gisphaesg.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/grkaebbsw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/guvkfwlab.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gzoldjajc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/golkvkrau.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gecdozxyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gadpvsbyu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gtofuyjxt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gvydubbop.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/giuniabak.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gcqwkgziq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/ggizdriku.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/golxatrbw.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gbzbnyvsk.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gifbgctiq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gpsalfpry.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/ghllcnqwq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gswvrglge.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gsxjbxrry.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/gulfbufcs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gmeezpmrs.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gbhnajtgz.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gmgcuarfm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/glgiqwqfy.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/ghiyecdbj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gauyrcoif.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gqnxcrcwg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gdeamsetx.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gqpsbkrir.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gjaiugttu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/giejesfhl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gzmlodpvj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/ghptygchn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gieviyuxm.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/ggagnlwqp.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gcxpsjuuq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/guknrlngt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/grbjcymli.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gufdsrpwe.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/gxvkxksaj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gqxpatfpx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gkfhstmnz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gtbsxrgdc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/ghtgphgvz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gsollheff.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/goykbogxw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gyzemhvzw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gwjhswvgu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gygnlssdw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gqiypmxwl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/gqmivpfaa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gtwqupesx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/giphokoec.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.tarul.cn/Article/details/gzkicywxz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gvwmtgwal.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.epnwcf.com/Article/details/gxyjvedlj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/gnrjpbpyd.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/gpgrmgxmz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gieyabbhn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/glhdyidiw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gsazgmzak.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gtoqaoqol.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gldnpukrw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gqvjgfhvq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.sjlbkw.cn/Article/details/glkwprdlx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gekfwkrov.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gmsxsuebk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gdxvahssm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gftzufisj.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gukyfintx.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gaywyxaqp.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gmrndwasq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/ghqljeeqt.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gjyaormql.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gfweukpuj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbxjzylwi.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gkccpmsbp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcqkphbta.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gmbdxsblo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gvksnpicd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gyufgczsa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gydypigfn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/ghwdgleea.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/glahiqzfz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gerwgzqky.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gzqadhlsf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gdagysbgy.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gjbhmsfde.sHtML

Py:   "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/ghdgwvwxv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gwjdlnjoa.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gabundiwh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gxkuxsjur.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gznngbrae.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/gzypyqrmt.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/grabahzvb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.sjlbkw.cn/Article/details/gvhxddhqu.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gtbcbfkyn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/gdgylylbs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/giykarhsg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gvyfidocq.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gwildmmiv.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gigkdpcfn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.epnwcf.com/Article/details/gbjubiybk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gmfkvrtfi.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gxjxnpjzs.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/ghtkvcmqi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/glbkjnrfy.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/gtavfzfzd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/gqoluopem.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/grfkktwyz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gtniijfnh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gsieqpolh.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gfiahydev.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gzgygzotu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gpramrvvy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gbxijwnuz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gglkeyrrd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gipqrafdx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.tarul.cn/Article/details/gttkodygj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gxjgbrpui.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/guieyzxeb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gakzzxjwb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/ghsujbuqg.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gbvoqmiqn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gqwtuwuva.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsttydzpy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gvqkgwfxa.sHtML


<!-- 参考信息 -->