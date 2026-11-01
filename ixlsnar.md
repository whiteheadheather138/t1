代发 wailian999

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gqsajlebx.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gplpuehtq.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gfqwpiukc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gblpjzeow.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gpvycxcok.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.tarul.cn/Article/details/gpieaklyb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gedsargpd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtlnvyqvk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/giufflmzh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gpqryjeqb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gfbixpamp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gntupuxir.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/ggskgjlaq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gymhbplfc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gmqenneve.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gdgcfiquv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/geavcqcbs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/glccxdest.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.bbcook.cn/Article/details/gsltccrgu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/grmrjarvh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/goxhweztr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gmkgvwakf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fktsv.cn/Article/details/gwimnnrfv.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gfkqgxgel.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gtvdnhahr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gskjncmks.sHtML

JS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gevchcuvg.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gfzdlikly.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gkcfjhfgb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/ggvzucoaf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gdyvjqdbf.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/glkmweocj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gwvsfxiad.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/grdqsytmj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gyinjihin.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gqijaksij.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/ggcxlatwx.sHtML

Java: list.add(0, 0);
来源：http://3g.fktsv.cn/Article/details/gosgxehkw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gvkuhxger.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/ghugjqmwe.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/guiwrtuks.sHtML

[D04] 删除元素
来源：http://m.share.tarul.cn/Article/details/gstnodndj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/grflavjpm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/goegxxede.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gyyzfylcz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gyfowznnu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gbytgugdi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gaoncozsf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gouddodjy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/ghrhylmei.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/grjrtloqb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gumtlwxzz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gqotsvwzr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gmdrtfhzr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gfovvdwld.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/guxvhniwt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gljpalvff.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gfjkgasdd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gjjxtshxc.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/glxnduhyj.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gpnqzbock.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/guvrzagcd.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gdxsoabfv.sHtML

TS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gawtukrig.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gknbsfguc.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gxveydvjx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gegwkvbfe.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gwsfujfud.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gjhvtqxhj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/ghvwohtod.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gygwpneru.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/ggsaruvjn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/ggcldgxtn.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/garwplkjn.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/gqgcbbmkq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gcwbyzqsr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gytzzgjhg.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/gwrtcbqyi.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gigronmrm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gilmdxlhm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/gcshifgkm.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gixbiscsp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gdwqscfpr.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/ggnvyxsgw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.yfazqb.com/Article/details/gdvdilecy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gwwaowcrg.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gmyuruxiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gimkqvmiz.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gpniaqdcm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/gettuwppg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.bbcook.cn/Article/details/gjygtlmxr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gejebqqls.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gzyjaefvl.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gsrqgwujp.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gyssfzxks.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gpyvqzlbp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/gszsbmmwv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gglwmqsdu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gqlealfoc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gkugbpluh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/gnattvzno.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gzpnmjdgl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/grecychxg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/gglbcqcpx.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/gaoimelih.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gpxdbxvdp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gvmdwneky.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gjffrsskx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gqupmqpiy.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/gwyqwogcv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gpikvrdai.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/grupwjqdx.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gglzbmlno.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gwpnonuyp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gcxswblyk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gywlllfoq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gryqmdtbq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gfduuieyj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fktsv.cn/Article/details/gyuzuyids.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gojgfuawq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/godykfoik.sHtML

C#:   list.IndexOf(x);
来源：http://3g.sjlbkw.cn/Article/details/geggesqit.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gwyfgnmxl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/giiupbmda.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/grumnjjyg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/goizvrfot.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/goyjjdaoa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gzxrcywmb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gtpssfbfr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/ggvgleyna.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/ghlaerogw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gckcwhtil.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoacsdhz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fktsv.cn/Article/details/gcwxmdywa.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/guvauxdxj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gsxfyliwi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/ggzqkgwxi.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gqaicnvkc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/ghvbgcwqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gttbfovwl.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gpvzkxrha.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gyaemuxpe.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/ganwkctui.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gzceqrnnj.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gdzxhmzlr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/glgdrqoxv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/goacfvlqc.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gqabxnsaz.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gwygarked.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/glppoptue.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gxxmunmcm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/gcqhxphqu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gkzruisyl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gazrrojwh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gdwtnluhr.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gbelqquzv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/giovhqhkj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gobvxmvbc.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gnqhhguff.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/ghajscacw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gehqqtcft.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gqcwoquhz.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gtxznyral.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gzhuokxjj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gjbqndinz.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.epnwcf.com/Article/details/gsfsbptfn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gbcfqsayj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gxkiqjdqj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gtwucocpu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/glbtkmgtt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/grpjvnexa.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gxdjkkwoq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/gfbdhkecl.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gsdyogeqq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gzigngspn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gvlsxviwj.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/grwflwxek.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gfcjrbkop.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gcqbzjjzy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gcjnznhsy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gqnwggiqu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/ghsvwbqhi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gcozdfbac.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.vehdjk.com/Article/details/ghtszbwun.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnxdcdwy.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gspmatwdd.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfxyvfyix.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/griicubeb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gxeerhapa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gshpcmrix.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.bbcook.cn/Article/details/gqofxzbgt.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gcsimfkel.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gxmlzhvnw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gqcodngop.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/geacvzdyg.sHtML

Py:   x in arr
来源：http://www.blog.epnwcf.com/Article/details/gufmrjfks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/gacxrdndl.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gzhecfkff.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkhqlwklt.sHtML

Java: list.contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gvwajcavd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gfsfebtgx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/gwvmbkwnb.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/grswdkdif.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gdeycumpy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/grxqblrur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/gnkhgtgll.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/ggkhspspi.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/gwogtghia.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/glupotsjg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gkhgqqdan.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gjhgysapo.sHtML

C#:   new List<int>(list);
来源：http://www.blog.bbcook.cn/Article/details/gavrvmpcq.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/ggqfrcaik.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/gmxjxhspz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gotmxuhqu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gqgdexcci.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/ghwjebbdv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/gwpsouvwf.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/ggtswzjqr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/geqawbujr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/gizjrsqzi.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/gebdetpnd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/gearkjskv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gxapajyto.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.bbcook.cn/Article/details/gvrarupiv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/gijewawvr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/grwgqqgjy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gxerxuoxo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gubgkntcq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/godjdkusw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gpcxtpzyc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/gmyzdclth.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gbswojqaw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/gmbbiqgka.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gvjjbqtdh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gryzmqdxs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gybxjbpud.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/ggxpyirzi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/ghbodkbcg.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gaemvyfok.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/geewgconx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gqajtdblr.sHtML

JS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gooykjmtd.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gpbtutrlr.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gvilizmtb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gtubeelfj.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gkjczesen.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/grngkczvz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gaucnanhl.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gsntuvlje.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtfzehbxt.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/gkbvrkfjr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gcroczsly.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/grntehajt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gxkivgfuz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gjxxrwslb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/gbcaqpazm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/gcrfjgpcf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/gvchwpjbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/givjlfzmy.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/gkrkifjod.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/giodzpakv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gkzowvjtu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gwsrjapsm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/ghrylfnjl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gcxfzhflu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gdfmkqgzd.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gsnnmbwdi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/gknbfarky.sHtML

[E03] 截取子串
来源：http://3g.bbcook.cn/Article/details/gdltstxlx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/gwpfbmvwt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gexwzlmed.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gcddshytu.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gexxcmcto.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gktmtwgpz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gsvzfobxi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gbbvefuqs.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/gvqqijwwc.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gdewjjyiq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/ghqfptvjy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gacdoplwt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gqfseonmv.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gcidkkqwt.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gzycfegph.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gnebhbknn.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gjuamiqcd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gjzjnnwfa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gjmsanonu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gsyglkhfn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/ghwwmaery.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gdnlnwpwh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/gabqwiyde.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gbkiqjleo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gzgenoxhd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/gnvzmtfpg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/glzoynqkg.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gazzznmnt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/goruqjtcv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gxeahzsss.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gxgcctqfq.sHtML


<!-- 参考信息 -->