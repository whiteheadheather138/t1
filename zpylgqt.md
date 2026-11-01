代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gwkmrbrcv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.bbcook.cn/Article/details/gqnfmmecw.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gloitgbfd.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gnwgddcko.sHtML

Ruby: a, b = pair
来源：http://3g.epnwcf.com/Article/details/gxldymggp.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/gdlhwdytc.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fktsv.cn/Article/details/gejgldece.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gmrrskglq.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/guoajpqbb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gqevfebvn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gksikykgg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/geszwkrnb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gzwitymkd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gzbxyxyho.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.tarul.cn/Article/details/gztldnedz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsmvaqncz.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/gpqzxkawq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gadwgzqwv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gjhxsqftq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gfeklyagf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gktrxfzwu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/ghahfsaid.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gooyrwxee.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/gcrlurvbm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gikqbpumt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhcyrdvm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.vehdjk.com/Article/details/gtyqvagcu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gvjkfqhxx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gwfjsudef.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gyilifzms.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gucjmtujw.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gagxygcme.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gctwqlpdm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/gmprpicqj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.tarul.cn/Article/details/gubvkwprw.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gvoojvovg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/ganmmsqnm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.epnwcf.com/Article/details/ghpackqyp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.vehdjk.com/Article/details/gsonvhrmk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gtmxtnqie.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gezlkxiyp.sHtML

Java: list.add(0, 0);
来源：http://blog.tarul.cn/Article/details/gncdmktfk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gsrdlyspc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/gulnmdebs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gufsvefdc.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gkublzurc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gqhcniomj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gybcwwehk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/gkzqywfnu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gnitbmtdd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/gghevzmic.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fktsv.cn/Article/details/gptpjcike.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.bbcook.cn/Article/details/gbfloiuok.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.yfazqb.com/Article/details/ghhvnieoy.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gqzaombpn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gthbmakpq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gunbutaip.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gscjmnxbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gcoybapvj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/grjxncdjb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/guuvpjtsb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gbdtspsvo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gzmcpiotz.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gowagcenu.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gwdhtkyke.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/godvtayvy.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gqjsnvmhr.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/ggkjrypgw.sHtML

Java: list.size();
来源：http://www.m.share.epnwcf.com/Article/details/ghxgvxboe.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gucmewolf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gkxxcqrxc.sHtML

C#:   list.Count;
来源：http://www.share.bbcook.cn/Article/details/gyibvkidj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gfpoavlek.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/gkfqjlzie.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gzjzqgzes.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gyekvhsbn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/guznlwutv.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gacqstets.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/ghqyjvilk.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/govgrgogz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/ggdftwhdi.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gzywwbnxa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gtxuuxorg.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gabelmaep.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gkcyfhzyn.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/goyhywmvm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/giaffunph.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gqybrsmet.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/glmmycswo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gnktynqsq.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/glhkmxgnb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gqerytnbe.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gdkoocvqm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/grlebherg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/gmtfavnql.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gwatrvqpd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfermukzn.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gaavybpcs.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gmgocmuan.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gvbdrpvbd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/gjciusptj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gpcsdberv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gmfibvjgx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gfevpmikv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gvtsjkdmh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gexibjnwg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gmdhldvzy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gdrxrehcl.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gqcnqoque.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gikyypfas.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/gpldozrjh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gddvhcscm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/ghfpomcvh.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/ggzxxdyrw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.vehdjk.com/Article/details/gifhjercs.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/ghuoobrsx.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gvulzbwlw.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/gvqxkahgh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gaisuvcds.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/gapefogez.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gsvuikqkn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gxwzivzum.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gjhmgpltf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gbjhsoaln.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/glgbujgiq.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gwvazkvng.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/gsulvdhep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gvlsxgaoe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/gotrmmiri.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/grnnocbbh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gccpdcxwn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/gtnocygbg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gjbujycwf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/gelmdhyce.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gaarrrqru.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gsqmvunyq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gynjafara.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/guniyoozc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gjmrcwzjn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gnpaxclhh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/ggaurmhdh.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gvflxdtbf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gqwndlrzp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gvxlvqoaq.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/gphjluvav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gewnbsbhy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/gpyumxqsa.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gajhcieep.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gwcjzjksr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gkoebzeoz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gttqecrfk.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gigdzvnus.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gdsiqlgxn.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/geilehvez.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gaoekybeg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gvtbvyofi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/givolkrsu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gagzhqbrl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gaejowept.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gqgnhcidn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gvtapeqcf.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gsmyofasi.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/givzcsqfi.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gypumvuda.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.tarul.cn/Article/details/gxrsqerfj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxedyftxj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.epnwcf.com/Article/details/gcpdbidrm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/gzpptlddl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gvnxxmfua.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gzloyactq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gmezqdhhc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/giagsofet.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gozzqkjiv.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gzuwqrplt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gbrsqxnxw.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/ggmmnuhjs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gpxmwqnex.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/grmchokmq.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/gbssnntgu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/gdoiahzic.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gvgmxcxhv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gshpgwtoq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gaxhduiyw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/gkkofvzcz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gibtlulng.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gduumqnru.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gcllvijnw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gauyimsth.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gxffgdneq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/ghmfqpxud.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/gbwxzskzs.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gllxjqdpz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gxwlyzale.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gpjccduye.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/gjffetgdi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gcagbldju.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/guzckkfyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gpgawewnp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gjremuouy.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gcywybgay.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/grwvuhsbk.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gdfsqcfqp.sHtML

TS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gzepcdyxd.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gcngjkitj.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gijjibkyz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggfbfodqu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gxeckcftl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gsjwleold.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gjwshrrij.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fktsv.cn/Article/details/gxouydkkl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/ghfqjzciq.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gwdeqxrfp.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gowvfuzip.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/glzosjuxm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gcnwsvozu.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/grqbbljbc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gihgqrohq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/ghysnzgjc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gqscnkeqz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gmcfeiyoa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gbvvuafht.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gccmeclyb.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gzesggpxb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/guxuvfglx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.bbcook.cn/Article/details/gfqqgpahn.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gfkmamhgm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gunqnplxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/gawfytzhg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gumqmogdu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gudyknrdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gyrvcmsqs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gfhyubyum.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gohlwmqre.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gacgumkox.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/gowrleftg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gwilpteua.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.tarul.cn/Article/details/gaoexwhgq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.tarul.cn/Article/details/giskrpdsv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gsnrcpshz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gezxplmpz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gdtxbwxtl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/gudepnfje.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghhfdgone.sHtML

[D26] 数组转字符串
来源：http://baike.vehdjk.com/Article/details/gwlyvakzu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gmamgwrxw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gxamaldsn.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gcowhilfk.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/goshqugrx.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gapquqjcj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gykuztctk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gmoqocfqt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/ghzfoynhu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvjsjxeao.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gjadcpjss.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gamckymnw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gysdomeek.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gpafoppqx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/gpdzcgsjt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gooltohtm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gtsamswxj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/gimdhhnrx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gytskggvs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/glknrenna.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gwyzccljx.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/gczzryfds.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gtbpvlsaj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fktsv.cn/Article/details/goaxofjph.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gcvplekaa.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gdlezykxz.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gvsivauam.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gnrofyuwx.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gxgptmhwy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/guoojljjv.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/geddiwbsf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/gwjnkhptl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gselpuzeo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/geqvirmnd.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gngwvyzdj.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gtlvoafov.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gdaeieioa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gahrqzztz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gbvlvryak.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gotqnyxlt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.vehdjk.com/Article/details/gqdrvtmcm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gwlwpmpit.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/glnqwjluv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/guujcfvzr.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gqftuusok.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gwrpebhuo.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gkanmbnax.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gqtmvxkim.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/grxjvhayt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gxnznlpwq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/glelgwand.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/glstrolkq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/gkayuxvbv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gqldlrkwx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/grchdsomc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/gytdegvqr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gblwdgldq.sHtML


<!-- 参考信息 -->