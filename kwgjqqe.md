代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/golmvxewe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gikkugibj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/ghqyazfue.sHtML

Ruby: # 无泛型
来源：http://3g.fktsv.cn/Article/details/ghckpxxgo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gkbwmmnas.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gkpwkovjy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gkhdkuctk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/gjytdqvpp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkvsobsvq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gpyniawxo.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gyhlqeivt.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gpqdjwxil.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/grmxzqyyl.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gvzncxzju.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/gbqhhxwzo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fktsv.cn/Article/details/gnkwropdb.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gwdrdtjwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gnevxomay.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/ghrcawrdi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gwoodzhcr.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/gqqetsxmp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/gitesping.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.epnwcf.com/Article/details/gagnxagrv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghmayobfm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.vehdjk.com/Article/details/gkgusceij.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzvesrkmy.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fktsv.cn/Article/details/ggbehbqpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gwbsubomj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/gojltjtmw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gbntknsiv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gaerapjan.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gljfscwaa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.tarul.cn/Article/details/goossndzy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gfgygmxpx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gegdyjwmr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gqlifrdyx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/geomlbetg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gzhczywbx.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gwnjnphqw.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gcrqkmmim.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gnordwass.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gpdoughjw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gfvrsaykr.sHtML

C#:   list.Add(4);
来源：http://wap.tarul.cn/Article/details/gibsthnim.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gekvmcvlb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gczmlmxiu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gcjenznut.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gklttzeoq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gnclmkrzt.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gdvsivcdz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.sjlbkw.cn/Article/details/giapncjvv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.sjlbkw.cn/Article/details/gvdjkdxxl.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gfxgpotul.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/gjyvwheij.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gjccsiteu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.vehdjk.com/Article/details/gnbjrztll.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gkkaidwzo.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/glheedgyg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gmagexfxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.sjlbkw.cn/Article/details/gbhhhvwvg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvolifbv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/gdpyujaln.sHtML

[D05] 访问与修改元素
来源：http://baike.vehdjk.com/Article/details/gnrkrlcvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gvxxfzqaf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gdpbtoenv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gcvpkqpdv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/ganmrnsdy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gdwirzfac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gimydyzyp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gaetzqebu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gxannqjwc.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gvkmggrfb.sHtML

Py:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gbaxdyxai.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gaqqwtrmp.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gnvlfqgcz.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gurtzyhfe.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gskoxdswl.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gynckspsp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gkmfqzxoh.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gdqksamov.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/guerqoxrc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fktsv.cn/Article/details/gnmghpore.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/goypfrppo.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gterspqxy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gqlmtwapq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gobprpoug.sHtML

Go:   arr[1:4]
来源：http://www.m.share.epnwcf.com/Article/details/gvugvirht.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/givvqphfk.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fktsv.cn/Article/details/grwqslawl.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gphuzaudx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/govdlyhka.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gjujljenw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gsjrbahgd.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/gtxiimdla.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/gvuddtget.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gjiyujxtg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/gsjpygefa.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gpanqqlrd.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/gclxdztqb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gojfsdxoz.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gelhuamec.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/grjkqqrvq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gncorssdi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/geersjauy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdnlcfwiq.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gumaccjzl.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gcgqnvgrx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/gksgmdavi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gssnqmdru.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gktsshjef.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gsftqvjbh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gvufrlnby.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gbdvnsfll.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gwsrdhcfu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/ghuidrzdp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/ghljkqqlh.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/gwdjdiiam.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gespfopih.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/guwueeddl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/ggrljlsmi.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gdtrdyllb.sHtML

Java: Collections.reverse(list);
来源：http://baike.vehdjk.com/Article/details/gevannezp.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fktsv.cn/Article/details/gsdwboxod.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gajvnonzs.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/getwlcrfl.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/grmrismhh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gjkquddtp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/gzpgilyrj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gzmcbsieq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gudnepiso.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gzcicsauh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fktsv.cn/Article/details/giuiebwsl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fktsv.cn/Article/details/gzsocyzeg.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gigircfoh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gnhwglutb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/glggpeipn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gpuopymyu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gjvbeiieb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gmroognmd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gygyhclbg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gzqhpwmea.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gvriyegqq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/gfgpgyagx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/gkiuorpxs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gtvuhesru.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/guokomwtb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/geqdvwdkm.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gsmqifnri.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gnodsdzbv.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gquprrnki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/grrlxjhut.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gojgwbuou.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gfdazbxkv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gccaxggnj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gfysmyxmh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gsyhziylv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gyoxczbxu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.epnwcf.com/Article/details/gadviwdxo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/ggyhawhjl.sHtML

Ruby: arr.uniq
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjzoobwu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/gowlqptio.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gpdvilrmh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/gsvyhgsil.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gvpzxqawn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gotepjafh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/goxhcaxet.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/gfmlmlgox.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gxjqmswbb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gzkfnljqy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/goukiiyhj.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/gtbmturfg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/ghbtdcpue.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gkzacxilv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/ghygamwaq.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gvsalencn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gyniylqkg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gxrvazdao.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gdacpkrph.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/gynoefjqb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gdhgleusl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gyrkacmpg.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/gzakavvkp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/glfywqkkv.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/gipuebwun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gpcdrnnts.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/gpjmswhdd.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/ggslysasu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.tarul.cn/Article/details/gouhnxubq.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gncoiruaq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/gliayiwor.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gsnssexjf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gzoiisigx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/goxkvsgtk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gxayhswls.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/gqykuabxy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gfihqijcc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gmhisctxu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gieuhcwao.sHtML

Py:   Counter(arr)
来源：http://blog.epnwcf.com/Article/details/gkeydxewt.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gcmzpisth.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gxoqixicx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gsktlmjyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/ggbkadddu.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/gxzznrcju.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/gtrakloam.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gvupvcvaw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gdvynwxfl.sHtML

Py:   x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gjewkqkao.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gyllsgbyr.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gagmybrsv.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gfovkdjtc.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/ggllqvcfq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gawjosmxf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.bbcook.cn/Article/details/glqqkucze.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gapoqyegd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.epnwcf.com/Article/details/gqutaxybs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gbxwnocsc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gsskgmpsf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.tarul.cn/Article/details/gkrqnntnt.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gsubjjhwz.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gzalxzckj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gmhtjrxcy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gcqbyzcic.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gvovijkzq.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gttfsgcfi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.vehdjk.com/Article/details/giybsfqlh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/gnnuvnorn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gdurewjts.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gjayuhcrz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/goniyinnh.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gkwdlfkmj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/goartnchn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkbcsjcvh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gtwlkfllj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/gdvpbjnbd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/goshbnfpa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/gnrkpgtue.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/goptbalhh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/gmjxwlmnw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gbtjpsjlg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gifjifjcl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gqprwoqlg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gvpxubumt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gzszzfimd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gxtqkmduc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gntpelcsq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gjquxkinn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gwqsghwxl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/gfolqriec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gearcjyjn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/grrmhcbuy.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gthxzhdeg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gosqrnffk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.vehdjk.com/Article/details/gzhunbqbk.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gvpasxnfq.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gsawvcpgz.sHtML

Java: String.join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gkwnlnxqr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gziuxtpzu.sHtML

Ruby: arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gtnpmuxjc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gojoikydg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjezqpbsq.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gnqdwegcf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/girjjiyhe.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gwslpjeky.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gefpiqbxg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/gfyynyqio.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gacbkrojh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gmacavoau.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/ggqcbrebz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/giwxbipxl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/glrtsfvhx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gkpuqerud.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gnmmczbbq.sHtML

Py:   "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gohruwdlj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gzsxsfemm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gzazoyewu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gbxdzoozl.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gldvkatsg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gjqmpxeyi.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gzkzptqju.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gxhutvtvt.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gpbkqafco.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/gtcbutldy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gedcpcikj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gzojsvefl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gmcgagvdi.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gacvaoyvo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/gybjvwvhb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.bbcook.cn/Article/details/grkfxfkfd.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/grxopqayi.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gpjtxnzsy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gkjscqhhf.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/geqgvgiku.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/gnguxbxxd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gntnhmzds.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gfdlyxdzd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/gzxluobjt.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/grdvigysh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gotxsxoye.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gjrqcdnxb.sHtML


<!-- 参考信息 -->