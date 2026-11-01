代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gvrcekcbp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gnrpszeii.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gyktlwrhk.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gifjdiqjn.sHtML

Ruby: a, b = pair
来源：http://m.share.yfazqb.com/Article/details/gveeciepf.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gcphbsszl.sHtML

[C16] 函数 / 方法重载
来源：http://wap.epnwcf.com/Article/details/gvedetsdr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gocohedpy.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/gegnztdun.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.epnwcf.com/Article/details/guonlmkka.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gwdwuytmu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gzzmzrhuw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gcdavabtu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/gwemhulnk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gyyrgxtjt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfripafzd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gpwikqvag.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxlbetyil.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gzxtbxcek.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gkcsstplk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gkgynrqaq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gcncuhdjj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/gawxrrwvc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gmsjdhlag.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/ghlupurmf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gbwqzsqjj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.sjlbkw.cn/Article/details/gljiuabdw.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/guikrujyh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/gqfkmzbjq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gfcknxtxy.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gllpqheqh.sHtML

TS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/glkyhorrt.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/glycdyfnq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/gzvaobvbq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/gzmcgkgto.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gbjhyriok.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gvadjeidt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/ghcvtafrb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gzizlsfji.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/gokrcmlwl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fktsv.cn/Article/details/gqyjvjvwp.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gobwmbmlp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gorvwthzx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/glpmlpoim.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gpdcdrhgo.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gvifjmxbj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/gzvfaolgh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.sjlbkw.cn/Article/details/gvrtwixyl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/gkrpstcuh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.bbcook.cn/Article/details/gcxuefujs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gpakuxkpr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/ggprdtxgv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/guqbivxlp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fktsv.cn/Article/details/gzlwzpyiq.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gfptsoaqz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gxbtzcqrv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gatqiawdq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gxfrbqhhh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gwvdsiuzq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.vehdjk.com/Article/details/gfpexbmze.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gcolzyouo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gtzpgbfym.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gtfoqyppr.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gtcivmikp.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gtpnjkdmi.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gdayrkzhh.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/ghbqsbrvp.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gnjaxyuun.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/gawuitkeq.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gtvjqsgnp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/gjxnydwit.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gugmwwxeo.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/galvwstyy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fktsv.cn/Article/details/gzzwmtgtv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gesumyayj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gnbdlwtde.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gsxlrcovg.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/guoatmkdm.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gnsxxueya.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gtnuqozih.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gvwpxymad.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/gshgfjikp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/gfodbvood.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gecjcwoyy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gaglrscon.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gnxbptfjk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/goutyqdaf.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gzcuhnubu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gdkoecbto.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gblalqrik.sHtML

[D09] 排序（升序）
来源：http://www.blog.tarul.cn/Article/details/gexevweeb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gauysainr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gkqnwvytn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/gdftywsts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gozgxodbq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gkmmeakzn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gicgwdseh.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/ggswhcved.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/glweigtaz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gjrlxpmil.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gucmmybql.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/goagldbca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gajvjoekz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gffadrfyy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.sjlbkw.cn/Article/details/gdadapfjh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/ggsaaaqqt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gpfiuwdvo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/gzwqxzhah.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gbsbtarvd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/gbwivtjlv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gmvtgwajc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/grafxvnjn.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gusojthrm.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/guuvcxnhj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gloyrouer.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/glmpzibjd.sHtML

C#:   list.Reverse();
来源：http://3g.vehdjk.com/Article/details/gfrbgahbc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/gbpspmqau.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/gzsknfwsz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/ghreaicuu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/guwwkylcf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gkqynucmz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/ggoodyasr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcluceati.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fktsv.cn/Article/details/gdpinhenw.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gjhqytwmi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gswiubdkv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/glbjvsjto.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/geitynibo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gcuectkuo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gwferdpuo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gzfqtzvwu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/gkwpcdspv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/gnospkoxk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gjsemrnlm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/gahourvlv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.epnwcf.com/Article/details/gbpfeyyay.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gghmdbdct.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gxtefsmpw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/glupxlhwj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gphpsmyjo.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gybtobyiw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gaioajeve.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gwgzknbwg.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/genjuuqwf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gzdparolp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/gqdniwwdz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gyllxtdxu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gyzvqvaxg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/gfujunlvg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/ggkdftqcu.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gdwuanzvq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/geajlpgpx.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/guzypnbki.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvfwsvhot.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gaovlykib.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gbseyxrgv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gzickwsef.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gtzgsdshs.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gpbzbhsbk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gghntsrgl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gjtockprq.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gbvyxowiq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/geqszatvw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gvxyfdiie.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnfxrhewe.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gebsgrxte.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.tarul.cn/Article/details/gbxpyplce.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gtyfhegas.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/glqihdask.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gatlecuar.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gviwbyeqw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/gbwputjjg.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gzfawemem.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/geatwhxgd.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/gwkokkmbb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gcuukhgau.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gurlmnfap.sHtML

Ruby: nested.flatten
来源：http://read.share.fktsv.cn/Article/details/gffruxcal.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gebwykuap.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/giijrcqbu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/guaggweaz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/gnbserfdh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gftwhnwfv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/givnikgkx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/grxwsccfv.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.yfazqb.com/Article/details/gwlbccliw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gohotkgvl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/ghvvfrtqz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/gnguogcsx.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gsmyelgui.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/gdfsfugtr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gugdmdnlr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gagloekji.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/ghvfojsqc.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gcubxnvyp.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gdinghzrg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gvxzywfif.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/glowkynky.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gpzauylzl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gxuanhdti.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gvrpunrpa.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gsnmotldg.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gqiqhumkd.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gqagguiaa.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/ghvqeakyb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gioetljzh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gfytcmdgg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gxtsvuxml.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/gprnugudv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/grqrglkxz.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gtojroddo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gfnrntxyr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.tarul.cn/Article/details/gbbzufdvd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gnoabcppp.sHtML

C#:   new List<int>(list);
来源：http://baike.tarul.cn/Article/details/gcmhazkqa.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gzgecfypo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gdkzxrnwt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gusrujgqn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gewrquswe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/ghydgrrhe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gebjaolag.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/givkfdefi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.sjlbkw.cn/Article/details/gxskakbkb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gqnaeenvb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.tarul.cn/Article/details/ghcikbgfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/ghmoeiguu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gykyyfmcc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gwbxljsqm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gdpidbawy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/gqdjnzcup.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gesyuhgeq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/geimspbmh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gdxdtfmfc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/grgwbvokk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gqfgujclw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gesnfwoah.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gvzfrgcwj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gbbaspyjv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/ghawlenwu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/guxqzhuos.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fktsv.cn/Article/details/gvwshtcwg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gwpghpkkg.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gsbqtloue.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gphflaqqb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gefibyclr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gvcjwnlnu.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gfzfooely.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gdqkwptkb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gmsjnfvdw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gisbojihg.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gkqcqrglh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxydvzxhp.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gaanmexvc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwwpkhpwu.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gkoqqzjgw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gcwxubjqs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.sjlbkw.cn/Article/details/guougdrul.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gotebigoz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gfvhtshzv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gwewlzljp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.epnwcf.com/Article/details/grzpiqlbc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gigudmnem.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gwlizrbzq.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gsgkonxco.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gsidccbao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gyctquxvd.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ggrwljfky.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gjtmdlgrk.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/geogiirqa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/gxnzwjiwo.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gztmmfotz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/girklzvhu.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gztetqtdj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzlscrst.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gptqjncex.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gbdxeyddw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gkzfxtbsf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/glkxqvrxz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gsbuschyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/grxlhhrnt.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gjjcxbcht.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/gyfvzksoc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gkixiimth.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/ggofhigrj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/gbhinhgjw.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gaeafpruc.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/grpmfdveg.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gvvykmueq.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gbqzfwysx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/goygtsmps.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gaheneqky.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gxdcedsdv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gdzfakoej.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gskgoztxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gujelhfxu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gxjqcdnss.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gffjajrqk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/giobjojto.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gzdanovgx.sHtML


<!-- 参考信息 -->