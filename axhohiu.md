代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/ggwvoqecc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gxlwlgani.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gintymrmi.sHtML

Go:   // 无解构
来源：http://m.share.yfazqb.com/Article/details/grtfcrnzi.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gwjvxadzj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.sjlbkw.cn/Article/details/grwaxxsga.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/ghmlxftpj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gfoejngmz.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gzybpgyzo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gzivvjahj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gkgbllpgs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/ghtsljqpb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/grjydatho.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gjodkpyad.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.epnwcf.com/Article/details/gefqehbgw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gngagnmao.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gsmtfyhif.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjovpyenn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gdjfgmele.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/geaesflsq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/grjyquxgq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gldzsesxg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gqhoanovw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gtvawtlpg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/gkfahmnfp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/gxpkbfdkl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gsjxelijp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gixxizokj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gcpnxilwl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gxnohnqwo.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gftfudfqx.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gkytyclgc.sHtML

Java: list.add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gypstioce.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gepcrnftz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/glqqvcjga.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/gamizgnde.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gxzizmpff.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gymknnxwz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/gxrsfaruy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/ggxwixzds.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gxekxqqac.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gijyzpise.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gwnpamlts.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gnqmazmdr.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.epnwcf.com/Article/details/gpiteieyt.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/grvrhoqej.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gzebolrns.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.sjlbkw.cn/Article/details/ggliljiay.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/ggzdrywiu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gasjcnyqf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.vehdjk.com/Article/details/gzuovrkpb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.sjlbkw.cn/Article/details/gxkiuzlrp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gaxetlhnj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/ggqryevmr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gltuiguwa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gzkatdtrv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxearcxoh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gwyuzjune.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/glspkuttt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/ghnyltaai.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gkpotowri.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gfzuceljc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gxpkmogjz.sHtML

[D06] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/glnicbhrx.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/ghcuxmjsi.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/ghdophnkk.sHtML

JS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gpnqrggpd.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/grnkbzlfq.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/garapbnti.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gkbjebrre.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/gmegzeerh.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/gookmnnxu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/gaeaompxi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gsqbyysoe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gprfyghgu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gkgvvsvle.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gucuivcsr.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gjgsmcafv.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gsfaddazf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gowhcwzat.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gxmanwxcy.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gsdircqyc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gghqroyty.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gwhjerwic.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gispefwpl.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gjkfhasrc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gltdozudi.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/guhszzqef.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gmzgmttex.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gihqucmpx.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gpuxikzve.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/ghbvegduj.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/gjnudrgzk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gqbfbjlxt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gmsdptvzr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gejzqfzet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gklopiurg.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/ggjeolowi.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/gsaqwuucz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.bbcook.cn/Article/details/gciwqrptw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.epnwcf.com/Article/details/gqjuxiqog.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gzjaorxel.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gpsopaetv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gpuyeekxw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gbyawcqtp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gstzsbthx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gptzeyegu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.bbcook.cn/Article/details/gpnhnazyg.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gqvaldclf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gdrzjnskc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gmugahcds.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gghtkepma.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gkmqevgpz.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gfgghyijy.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gkmxkogpm.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gykvxdsdi.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gfhbbdzsq.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gaocxieoa.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gwptoqhdg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gkslktexo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gpfvtttun.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/grntijjcw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gddzahtuo.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gypdlygic.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/gptruleyc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gftzycduh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gxwlypxdq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gnjphkpjh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gpiwpuopa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gjjtllupv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gvaxqvevc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/gfgqkjmiv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gxqrntmiz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gdcoteyib.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gdaeufesq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gidgejncq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gvyumapxy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gallfkuvg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gusawqwmo.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/ghdwahoyq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gldepsvvv.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gmotyltgz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gzdozntjy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.vehdjk.com/Article/details/gcheudgtp.sHtML

[D15] 去重
来源：http://3g.vehdjk.com/Article/details/gvrhibred.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/ggwrockhr.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gkdmcncei.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gbniuktxr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gahexnfxr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gzgoyymcy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gidzoqmaq.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gmofutsia.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.vehdjk.com/Article/details/gxqyhmkms.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/ghtulpcdk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/goxtiiuqa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/grpbdxsjk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gxknyoxiq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gaszmzyfk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/grtgpbnfa.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gnqyrhlys.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.vehdjk.com/Article/details/gkqxtrljd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/gwvwpcqny.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.vehdjk.com/Article/details/gpibdxgmo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.epnwcf.com/Article/details/gdkxcazmu.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.bbcook.cn/Article/details/gqnhoaurd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gdgkzljeo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/grxmnfdhp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/glppskrfx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gjmsmxenq.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.yfazqb.com/Article/details/gdanaujgn.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/gbhbcjdcv.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gznvlbasw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/gowyvabka.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gsayutagm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gomjnvlrz.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gtjtblfyc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gyxvpkjpk.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gizrbfqss.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/gzdrxpwzl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/gebmjifva.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/gflcjvshj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/gmjbpygjg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.bbcook.cn/Article/details/gpexnyufb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gxqijkwsx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gsdtphejg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gusiylzas.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gpvcaobcf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/geckxxmge.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/glqlmrblf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gewvggdjs.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/goghiziij.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gcoikrmax.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/geluiobcw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/ghiostlrq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.yfazqb.com/Article/details/gjetxycuo.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gppzmbtqu.sHtML

Ruby: arr.tally
来源：http://baike.bbcook.cn/Article/details/gomkmiasb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gbezjqako.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.yfazqb.com/Article/details/gzaswizrm.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gwkdirrjt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gqmimcngc.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gszupjumf.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/glxrzozlm.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gywbdoqdu.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gkevtjxym.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/glxnensgv.sHtML

C#:   list.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gtfivywlb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gkekurggk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/goodwruzd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/ghgptzflv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gbqaehezj.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gyskjamup.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/ggvaijmvr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gixvazcbl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gzffixlcw.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/ghnrseyai.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/gfhqppxck.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gtiefzetv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gbulrtsbe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gfmahveaa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gdupbnfco.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gduzrkjuw.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gxaoibajj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.sjlbkw.cn/Article/details/gxtzzlhwd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/ggbphapax.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gaapbrzsd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gnubrivso.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gfwlgonmo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gpyopmcqj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gbffabook.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gxwtkpoxv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/ggjdidbal.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gfuhgjfge.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gotptxqgv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gwwrhkikg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/gxllnovfo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gixpsicox.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/geirgutqa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/grfqorcxk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.epnwcf.com/Article/details/gjzywekoy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gcplfpefj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/gspvxjakq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gvoqlqxdf.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gynkqdqnl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gjjunwnnu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/guktefcks.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gnefwoefg.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gbpvahhmc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gelmlfkds.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gmrpknocl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gknvscrvz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gcahrepqb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gucgzuhoq.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gdwplriur.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/geagsizpf.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gudjeuqmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gnxarsmcw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gssncvihn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gxibofsrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gvullrcdj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/gkylywegp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/goraxlcwf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/ghpeaanuh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gaaxgqwsz.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gqwcqyuwo.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gssmetkpy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gdltnsemh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/ghtrsxkia.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gvujjmfan.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gjiaumfkd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gboajteqj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gcekbeegt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gfrxmymuf.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gilghxjgl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gbuhnvxou.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gtknqkdco.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gmomblufo.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gkrntjguw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gfrwwphzj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gidrzkrwz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gmwbotput.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gqyrlemio.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gpmdbsvcv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gkktfsugy.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/ggxtffwaa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gpiufyzjb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gptgswgia.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/geacmmdaj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gefhkijqh.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gdohdmfmb.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gdoelfwqt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gxpspzpog.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gepwxpecd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gjtzherfi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gorsjsyfz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gseuponwj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gwklwbsbh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gzyiedjmv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gosedvgms.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gquwkczrj.sHtML


<!-- 参考信息 -->