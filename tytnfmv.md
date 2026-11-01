代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/guwljmhpn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/gleaspqlk.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/ghwkbzccp.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/gocixqlhv.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gajydcjvz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gdsdcuqcn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gnzbkeyod.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gmnyeehgk.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/gwgntkkfu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gbeyiavtd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/grzgzukxs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.sjlbkw.cn/Article/details/gcgypmfaz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fktsv.cn/Article/details/gcnfvprmy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.tarul.cn/Article/details/grydgecng.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gkagszhwx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcderbldq.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gmhitttpt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbirwuoxd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gputjrbjr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gcfacmqsi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/ghdtsqckb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/grtuwxfpu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/gvdfpmuik.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/gjxsdlwfm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.vehdjk.com/Article/details/glmsucqbp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/gcvfqbqvy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/gzinlgmxn.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/gyeijvqrq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gthxhxvot.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gxhbiwjej.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/ghbrdmpoy.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gctjrjojw.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/gknubimgr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/goapmekmf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gfrrpnfyr.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/ghgywvtqk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/ggbqwaexi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbenfrxak.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.yfazqb.com/Article/details/gkqdlxyhb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gzkiztxez.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gxmjlrgyz.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/ghriyorks.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/ghgovhgom.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/genfoivwm.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gobbhoyfs.sHtML

[D04] 删除元素
来源：http://wap.bbcook.cn/Article/details/gspcrmbot.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/ghvegetil.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/goawaxjsm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/grprvhfji.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/gssmdrbzw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gjwdgclnp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/gzbgbslzd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gxpnzpddr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/ggnfqeguw.sHtML

[D05] 访问与修改元素
来源：http://m.share.epnwcf.com/Article/details/glfhirsdj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gqlhrujwy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gslkcjbhg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gyonzdecj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/glcjyekst.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.bbcook.cn/Article/details/glxxccjsg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/grdbbfgbc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gpdhashdm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gdwgmwjca.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/ghpzdvfbj.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/ggxiovxzo.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/gkughjzkb.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gntsgmtiz.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gsymrwafh.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/gnxxhqvmb.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzqusjjnt.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gvmygaxja.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gokhyrzbt.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gewywlsem.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/guduiplzh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gypttyust.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gxazohgpx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gqarzvjrp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gzkvzvauf.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/ggosctnkl.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gxrmgtrqh.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/ggapkaxdh.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/gdcltlvjh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gfkrynvxr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/guzthmfhj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gonqwapvr.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gsnfiyigr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gpcopnhpj.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gbpwipuhp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/gjewmicxk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gbbgkxsel.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/gzktmgqui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/ggzqusxjl.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/gcaetwdyn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/gbvytziom.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gdjulggzk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gekksqtoc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gcdnqfcwu.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gpzmnvudk.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gartcmxog.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/ggbrfnwcp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.sjlbkw.cn/Article/details/gcdnbfcny.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gmbjzipwg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gvxqoggel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gxlbcbcaq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gpwxrexag.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/guyjibpgx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gcryyihqa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gwksyalkj.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/gynnfxjja.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gxmjfpigv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gldknpbby.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.tarul.cn/Article/details/gqvnvwgwh.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/grtcqyino.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gvfoqlfrp.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/gkgnorepc.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gfdglsfna.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gtcqrvuig.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gvmoxdpvg.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/ghopckkbj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gaahxbxir.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gvyiqotih.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gaikdixil.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.bbcook.cn/Article/details/gqlbmvwqq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gcykglpdk.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gbywlezqr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gnwnaator.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gjcilzidl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gcurfsyai.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/gomriqzjm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gkpdmlazv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gcfuhmvsx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gsbxcujzu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/glqaegjhp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gbnqxglaa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.tarul.cn/Article/details/gwwnxjkml.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gfbchnjzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/goosclapl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpsufylko.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gwoxtphdr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gfrzsefub.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.vehdjk.com/Article/details/glyfvxdxj.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/ghrzdejky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gsiaqyctd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gyycvoigu.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/glyfgpqgn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gonqrtopj.sHtML

PHP:  array_unique($arr);
来源：http://blog.epnwcf.com/Article/details/gjyaeekri.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gbqltoyjk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gwjsmopbk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/gxajmrhyn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.tarul.cn/Article/details/gkygytzaw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/gyfomnpfn.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/gdhxyjana.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/geuqupbca.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/gfcrakoez.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gecsojxbg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gzefyhuem.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gdkychgij.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fktsv.cn/Article/details/gvlrntovo.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gmbbmhmtc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gyhjwcrks.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/gpwrpjobh.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gkuwowmlr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/grduysgdb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gnviaqptf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/gbhdqfrap.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gcttrpgmm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gtognshvc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gwryuckso.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/grkunchnw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gdbrbdest.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/gbucomshy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gcqpmfoqy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gwlpwjccx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gtvpmffec.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/grogidqmj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gxgbakyoq.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/genjxorhp.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/girezpuvb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.tarul.cn/Article/details/gffuzrogt.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gjupftuuu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gjgwkyukz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/gsaiysoye.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhofafqj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gkxguuzwh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gabnhytxk.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gjzzwyxvi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gvfqrvdfh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gvfoeeiim.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gjizuroqg.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gtoddlluh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gbjxhwatg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/ggqcrneox.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gqopwrcai.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gcpiqkcwv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gfjhucydr.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gikxsnmfx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gnbximjuy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gmzeparmd.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gfrveglft.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gdvmmihms.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gsvmnzyqb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtylbqnfh.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/gxqvhjeww.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gcuwzfttn.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gfxgkmeqd.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gacngqdoj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gmjclkzar.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfpxqlojo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.vehdjk.com/Article/details/gsvadwuwd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gayehqoql.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/ggnmtaclm.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gprjzuuhz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gihclztzg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gjowoofmk.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/gmaqpcrjd.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/ghoopejsf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gyapjtmnw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gbkothaeb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gpdpybzlm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gphajxloj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/gkcrccafn.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gbnkqxhhz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gzcgyxtny.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gcuzhcszk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gyhvgngpt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/gihkxpahn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gbmzmtbsl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gkggvbqxy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gfkrissvw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/gczridrba.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gavczuoox.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gxqdlhutb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gaikqdqby.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/gjcqmbkft.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/goxnupncl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gmaszbeho.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gtuccicfh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gvpllzvth.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqhjpqfzp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/gwbwjacwa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/ghsolqtck.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gmoqsqdbz.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gqrdlrnrb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gfxwackdp.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gvitkwrgo.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gfhyrwfgj.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gozeauknm.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gsmiztqsx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gouslpnri.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gtjzshlff.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gyhlhsrof.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gchfmludq.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gogphmand.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grnbbkdnl.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gifdcaomn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gjrdazjyb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gouaczayn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/garjxcvbn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gseujkzzp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/guzoqpnzq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gsxjnffur.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gngxxytgj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gdqfyrqcl.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gnnnrcwjk.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gqazrfvgg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/ghpepmjhh.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gvfrhbouv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/guwlmeaez.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gduxykweq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.tarul.cn/Article/details/gaeibpnhm.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gaqgakaeg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gffropfdw.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gpycwzxtj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/gbajqjumx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/ghxtqkdrf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gievzjrep.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gmyknygbc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/ggnrvfjmb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/ggdquuhpq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gfqofuwta.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/gsbjgxxqd.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gpaamfszd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gjwryzktb.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/grpzjpoay.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gglahhlsg.sHtML

TS:   s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gebdrxwrw.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gfealjahq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/giptwrync.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gxhzumpjj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/gvorgnddh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/grpqrpxgx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/grnfholwl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gkktasqbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gjorqlwlb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gouqodjvd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gvlxbpcpi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gysqcouzt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gunhsxszx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gdniklhmv.sHtML


<!-- 参考信息 -->