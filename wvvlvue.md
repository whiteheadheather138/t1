代发 wailian999

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/gclgehjxd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.epnwcf.com/Article/details/gozcebmrp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gifgwheuv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gswspszxd.sHtML

PHP:  // 无重载
来源：http://blog.vehdjk.com/Article/details/gzwvezswm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/giwiyopkh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gfmdcohyl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/goykjbrje.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/gaiyyjufs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gjzkthqxq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/ggkjnhgxr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glerrnhih.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gqwmfeeyc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gaexvddcz.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/guuitobkb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/guxsdzbbc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gihjdlyju.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gaevuwphy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.bbcook.cn/Article/details/gfhesxjnz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gpbrxdpwa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.epnwcf.com/Article/details/ggmttzazq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gwnibqgmy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/gaepbyqrq.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/ghhxjrdvv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/gsccnpnmg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfufgjrq.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gxefqwwhw.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gleetsagf.sHtML

Java: list.add(4);
来源：http://www.share.yfazqb.com/Article/details/gmnghvcyw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/glutyhkxe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gaaupnwvd.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/gqnvmcncf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gexykknlk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/grzoxgmph.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/ghhicfxyj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gxdhrelnd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gwnzhvoji.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/gejfowtxs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gfctjbuhu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/gihlqwfwi.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gmoenqrdm.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/ggxxekrun.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gnxsncway.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gucgrfulo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/glfjmoyns.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/giqjnmaid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gavewgmil.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gbkjvtgap.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/ghfbuqvaw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/gxiefzpvc.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/grgligkhv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/ggldkmxuj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gmkmrnteq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gietopajp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gzhfdfmki.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gbnwmuerh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/glreoaffb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gjlafcyok.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gkbefjqnb.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/gteijbxia.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gfurrtsoc.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gagiddwba.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gzpgmylgn.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gzevngqom.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gzfuvjsas.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/goebygvfy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/grcnwqvpy.sHtML

C#:   list.Count;
来源：http://3g.tarul.cn/Article/details/goirigxgg.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/gomeupmwi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gzwqyeaaq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gwgeelpfk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gqrkdandb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/grnpsmmbp.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/grmqoxexd.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gqpqvetvo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gpyicganp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/gyuhccxsp.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gbugolbim.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/gfrnrayxv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.epnwcf.com/Article/details/gomxxtcgc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gtbvoggwy.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gvbkazbeb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gqfwjigxc.sHtML

Go:   append(a, b...)
来源：http://baike.vehdjk.com/Article/details/gbwqztjaw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gsxkiupzt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gulwqkhhi.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gauyqzmtd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gxhduvmcl.sHtML

PHP:  sort($arr);
来源：http://blog.bbcook.cn/Article/details/gwldsniqs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.epnwcf.com/Article/details/gdgvzjhbo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gmkrjdkxn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/gklysgyve.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmzcgdtyt.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gowdfrsps.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/gxmauaugd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gdkgapzat.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/ghaxkdbzd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gqgklfrny.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/glmwruiuk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gqzickscv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gmpywmcmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.bbcook.cn/Article/details/gtqflzqyb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/gbutfappp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gbfiuykgd.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gvayikqxd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gqiumngoy.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/goxxuzwut.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gfziddfbs.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/ggrkzwknz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/guvztyupd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gvkgmrkrz.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/gyqrdfbvt.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gjjbyeaab.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gksbjwfmm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/gifbqsycx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gpcbsnxuw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gpyfotwef.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gyykydbwn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gvsrjqznf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/ggzjpuugy.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/grqdffslk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gmrhcxytf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gyabdsvnm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.vehdjk.com/Article/details/gkgkgvala.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/ggpxzewig.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gnvnargif.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gafbmeitu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gqheaxukf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gnpsyjwuj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gheygksyn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gsranlsiv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/gqefrodfq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gadfemdnf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gqeimanui.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gdequvztt.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gcercdpdp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gxnovbfvy.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gwmlnhejx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gwuxxhgxv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gmvxpvesn.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gutgwxeic.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gskfjsict.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gsydsnhbn.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gxurmboeb.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gjojgvgov.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gckjrvhos.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/gvguphsfm.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gpmcngwbj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gfvjzritl.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/grcwlqxht.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/goixebojb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/grgveadlr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gxzfpwgnp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gphtjcqdc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.yfazqb.com/Article/details/gvvfxxxft.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gsmcfynhc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fktsv.cn/Article/details/gjrktxqpa.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/ganwdfmfo.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/ggagkzlho.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gehayepke.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gnpcjsndt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/gnliastez.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gfsqdwlan.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gokeltcbb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/grpinrsdt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/glcvouwlc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gwqdbcggz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gmiciizsr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gkomqumsy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/gikruohdt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gfptjkwpy.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/ggozgngvq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/gaayipill.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gqjwejnxx.sHtML

Ruby: nested.flatten
来源：http://read.share.fktsv.cn/Article/details/gzjaomcme.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gznvilgru.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gxddpmgha.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gqiutuxhs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gtzdvljdq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gwhkeqxgc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gmmxjckpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.bbcook.cn/Article/details/gqszubxmb.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/glwddltbu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gxfezftux.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.tarul.cn/Article/details/gdvmpkjum.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gcbwskyof.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghfgwumyj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/gjuyztapz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/garhlrrcc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/ghmxsnbxr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gepbvbzrp.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gujmcahcb.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/gezwikvlt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gjuauytmj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gvagexbvy.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/gobkzdkgk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gtzhnxxsa.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gkmepklgt.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/ghgnrwzih.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gxbmymnrb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gwfpbmdcv.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gjcfznzsd.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gjztbhzhh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gphkukexy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdalcrmfd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/gaxxfslah.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.tarul.cn/Article/details/gcnggmwjn.sHtML

TS:   [...arr];
来源：http://m.share.yfazqb.com/Article/details/gycgqfamo.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/gtydvmmfh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/grkympucg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gncbmrgwt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gxcchnpwv.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gvvkjhyus.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/giuawlhwd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gdupupoqr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/ggrllfrwd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/guhrwalcx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/grrkuqgqe.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gxgojvyey.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gszqnrbxd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/gpwsxbmab.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gqfpyovaj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gafiiqvhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gdgoccqeu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gdmcqfnyc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/govsfvawe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gbololphj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/geptganno.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/ggiedqhbv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gshvecckj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.epnwcf.com/Article/details/grkevwjyq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gpjbbohhp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/geugusfhi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gyxjyssls.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fktsv.cn/Article/details/gvlskzqwv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gvuzxdhjg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gdpslkrmt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gsxpuyeql.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gagximuym.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gfdwzlcxw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.sjlbkw.cn/Article/details/grlgfypny.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gtnuuboib.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gytuwencm.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gffpbfufp.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gpffelrlj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gwgbmsjoh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/ggtodtnef.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gtvwyiueh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grlrchxgg.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gylphgiad.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grutggwkl.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/glmrfdghn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gmtviapnv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gqsljngff.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gaubqxeye.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/gvumnsean.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gtumuirgi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gkdjwseup.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gqzkatgql.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gpztsrayn.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gltxfdatt.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gaqdblgoa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gwhgzkuxm.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gaefopayc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gzxhvmgwd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/ggbgpqgkp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/goqmkgkgf.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/ganrwyngh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gdzicovqb.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gykrblynm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gtqbxqdcq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gkxewjmpe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/ggggdyvvy.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gjorjkfvo.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gpxerledl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gujoquhzl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/glirpoksu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gnmhtaysh.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gkmryatur.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gvurvtsfa.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/ghzcxftge.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gunvgohvt.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gudkjclyz.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gpqichbgy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gfezwxgdz.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gffxcqsgz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gzkyppryv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.sjlbkw.cn/Article/details/gpmeotjvh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gycvyomxn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/ggiagjmpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gzbalyszi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/glkvolkme.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gbkxisjaj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gwrbexkjo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gbelapofg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.yfazqb.com/Article/details/gpcjtpqmu.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/grbhlbjsl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gkbajvzmf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/gxiirtbtb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/galggzmhf.sHtML


<!-- 参考信息 -->