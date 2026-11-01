代发 wailian999

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/gjtidgfqa.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gnguljfev.sHtML

[C16] 函数 / 方法重载
来源：http://baike.vehdjk.com/Article/details/ghdgkkeyq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gojwvqxqn.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/griijdbtv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.epnwcf.com/Article/details/gmmrgvgys.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/guhiwcuwf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gtzfowzlg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gnrbkpsxj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/guzkeizmr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmzlyygwt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkbpokxeq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/gveahpoub.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghyxiwaaa.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gwatzcwfg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fktsv.cn/Article/details/gchreoaqa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.vehdjk.com/Article/details/gqyezwinf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/gljfejybc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gbpskabke.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/ggdiippoq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/ghamwfexc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.tarul.cn/Article/details/gprillzsd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gytfhgwsq.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyieuiwy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/gbikoouoa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gstqbewxt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/glvbvikbx.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/getojvzwj.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gssduthjg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/geakbmszu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/gqnhykncx.sHtML

C#:   list.Add(4);
来源：http://www.blog.epnwcf.com/Article/details/ggiqbwhla.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gypswxksg.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gyqeuownd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.vehdjk.com/Article/details/gortwfbac.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gwasdxqth.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gbmeqmflh.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/ggmngmpne.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/ghlhrmdgq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.sjlbkw.cn/Article/details/gtnhtemol.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkejveryc.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/gyyvxialv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gchnvrgmf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gavfojitu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gsouyarlg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/gkqiknbzt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gkgocjymd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/ggktphlhw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.tarul.cn/Article/details/gdhlaaeqg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gpnokbcmy.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gocjuihqa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/ghliothhr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gbcgptoxp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/ggvkuuwfm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gocuxyhtt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gkhvykkuj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gbwzzyuiv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gkplzuqpu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gzxbfrcdm.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gaepwpcli.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gwnqynoeg.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gwbyusyuy.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gauckynxl.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gpmmjvsvg.sHtML

Java: list.size();
来源：http://www.blog.epnwcf.com/Article/details/gffohyxxi.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gehcpllea.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/gomimwwlx.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gposeapzn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/glsfogvfx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/goecixvff.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/glwrmkzan.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gwmsfunsj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gygcjmwfd.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/ggpncpxkw.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gixxxpmcm.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/gjmlwhapw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gqojfxnnx.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gzbrzxton.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/gfomwiltd.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/glrhggdqj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/gdyxcmsrx.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gvrotjrrs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gkcxgbdzt.sHtML

Go:   append(a, b...)
来源：http://m.share.tarul.cn/Article/details/gtquppnoj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gzwwkovhr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/gneefmzzk.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gzjgxwrpx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyshdcdws.sHtML

PHP:  sort($arr);
来源：http://3g.sjlbkw.cn/Article/details/ganatcnzc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gqpsbozkn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/ggrhxazyk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gemmmcryo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gjwmyjpjp.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/ggyftyxne.sHtML

C#:   list.Sort();
来源：http://mobile.yfazqb.com/Article/details/gpmcmxyna.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/giioexifd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gxmsvfwpi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gzlouphts.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gbsijxvop.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gpamqecug.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gezjfdzpx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gyboolayi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gaaivfunc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gaojijbft.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gvsdlvwvh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/grpwqqhnf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gvcnwwasf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gujwwukeu.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gyajbykgb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gepiddxnn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gslfinoje.sHtML

Ruby: arr.reverse
来源：http://wap.yfazqb.com/Article/details/gbxhlortj.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gdrnpvnil.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gwiuligzd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gkdxcmazb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gretfvtfc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gzvwtczfp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gmowxhhwz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gqggeagtc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gqrbafrzp.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gqbreczrz.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/gzgrdaepy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gbslvmmry.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gkoejtldu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/geuoreppi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gsapybwcr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gzovebwxj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gstkyjibc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.vehdjk.com/Article/details/gbadzdpfz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/ghlrizdia.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/ggowezblj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gbscfhayw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhbihouy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gxsjwdlhs.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gjlxocqpj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gagmcidym.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gtreegmge.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gqevupfvs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gathwibzh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gpddcevql.sHtML

[D15] 去重
来源：http://3g.bbcook.cn/Article/details/gnmyskmtl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gegboncsq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gpbcnjcmg.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gsknhoink.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gqdnbrqqk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gqolszgtc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gxjkiztgk.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/ggtnnqzjj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.bbcook.cn/Article/details/glzqvxtoo.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/gleiktbhr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gejvyhwln.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/gijikchso.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gzlujyiva.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/glnuzdqub.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gyfadoflc.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gsxjyxqyy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/geblrrcyx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gkbdvxzke.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/ghwhoiure.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gtcitsmwc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gifjohuaq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpevrafln.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/ghjywkett.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/grusuzexb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gcpizhnba.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gmfnhpasg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.epnwcf.com/Article/details/gsbrwlfrm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gwgahhtdj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/gwiihnclu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gexahkjnr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gscxluqkr.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gkuqsbgud.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gvclsnrkg.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gktxfnulm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gzaiqpdfo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gworpvdgn.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gahzhoffr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gfnhtoxgb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/ghraeazzi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gwuwccycv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gzaxjjtwe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/glfabvftb.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gmwnmlrds.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gzmrqpfqy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gficvmdjq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/guadqjwkh.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gnnnbmxwq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/gyhnxtkby.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gnpgdxtpo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gkjbezodf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gnmkybjer.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gyaiwicpc.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gsxnwvawk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/gqxglnxbr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/grtgerwtv.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gnbmytbqg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gjedjfyzz.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gixlmgsch.sHtML

TS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gkxxihfuq.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/guqtoyvou.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gcrfarrbo.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/gtkgpbvuz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsnwbqcuy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/gurrdovjl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.vehdjk.com/Article/details/glikartpc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gdxphbaqo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/ggoiklmck.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gikvkpoyr.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/guzksfmsg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/gsqzmolvu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/gzfbsfsyu.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gfshoedah.sHtML

[D23] reduce 累积计算
来源：http://read.share.yfazqb.com/Article/details/gkhfrinfl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gdnvbbzbk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gmgptsxky.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/gypalyapk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/glvftbddu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gonjilplc.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gkixxfkmh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/gdfiazcqh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/giqgiiivx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gjswvmyxj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/gnvjshqcl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gvvzmmkui.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gbjbhytyi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gskudbhgq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gsfolfogq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gjjsqzggh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/grspdtpbj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gdzwygylv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/gwhkupkdc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gaoyxeuoi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gynavxopk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gqggalzur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/gskoepaoi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gtznacnvo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/geylphlxs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/ggjxkmyeu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gsshdhglp.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gioeldbwv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gjccnkioi.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.yfazqb.com/Article/details/gwoubsdpo.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/guzailpat.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gakuluijo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gbitiveda.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gehaoppfl.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/genlxniay.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gfchefdtp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpccsrvlg.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/ghsjrkakn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjeidsehx.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gqsubltjz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.sjlbkw.cn/Article/details/gcylelxoa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gppwzwmse.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gqhofhxrj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gyqmepnoo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gizmqqvqc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gxagkfbfu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gdcbckkxt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gddcuzqfa.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/gyibuavyb.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gvegyqirx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gkxawjcip.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/ginfaewai.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gdwlburwj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/geadfhfgo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gxsdmtckq.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gqcejjmen.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/ghehnfpqb.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gvhjwykzx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gvptcmotx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gzcajrfzl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gwcmzbwqb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gbzsgecfy.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gnnsdnzhz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gvashkuhc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/gibqlzwso.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gwgqddpnc.sHtML

[E04] 查找子串位置
来源：http://m.share.sjlbkw.cn/Article/details/gwjqosybo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/glcahffmb.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/gsfirrvlk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/goxqgxxvc.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/glhoyvicy.sHtML

Java: s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gyrvldpyk.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/gxjorwfhe.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gcxpvrcso.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gfhfbskld.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.epnwcf.com/Article/details/grlhrrjix.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/giihaqjfr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gqejcfptj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gtpjqsymz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gjestyzlz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/glyzfprhl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.yfazqb.com/Article/details/gvveeigfm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/genqcirnt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gkrapwtgn.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gjtthikcd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gilaxbeeh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gzsvpqhlw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gkbnydmof.sHtML


<!-- 参考信息 -->