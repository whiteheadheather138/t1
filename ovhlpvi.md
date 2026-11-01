代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/ghjzrycgr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.tarul.cn/Article/details/gngqdvsmb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gpbhulmaj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gybcyrayy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gdmnwpyys.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/geumsayxi.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/ghpfknuif.sHtML

Go:   // 无解构
来源：http://wap.yfazqb.com/Article/details/gfhchifjq.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/gmzptrmmi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/guxwgoqgo.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/grnvlafaf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gaxtbmhkh.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gfkcmrnhx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/gzorugjdt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/gxqshjxie.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/gnzyvvifv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.yfazqb.com/Article/details/gzofhkdkp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/goobztgxs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gyjumakjd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gumbibaqd.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/gkpijsxnl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glfqlsndn.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/ghxmxmyyi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gwdaecdsu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.vehdjk.com/Article/details/gswrrvuja.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gkcogcvsv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.sjlbkw.cn/Article/details/gtpcecqnz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gznzuotcz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gukmajrtw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gtutsxgoc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gnixflzmd.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/geendvhci.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gdtrymgew.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gunbhzaig.sHtML

JS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gtgnboyko.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/glccdfmcx.sHtML

Java: list.add(4);
来源：http://3g.fktsv.cn/Article/details/ghksibnso.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.yfazqb.com/Article/details/gbigosvyu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gxeztwfvk.sHtML

C#:   list.Add(4);
来源：http://blog.tarul.cn/Article/details/gzubtdoja.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gmjrpwans.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gsgwihhrc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.yfazqb.com/Article/details/gfxtxyyue.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/gwctaczzz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/garrkwnif.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gkxsfdyef.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gzrgshmar.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/gtcbroamv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gtvyawuyz.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/greybrqep.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/gmbawcbgz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/gpdtnymax.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gmvzkfhym.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/ggassxgzc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.bbcook.cn/Article/details/gjolfoitl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gwowscqlf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.vehdjk.com/Article/details/galhjbkwm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gdbdzgcgd.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gldbrreay.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gzoazhicb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gydmjfuot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gxhgqykhh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/gmjgqctif.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gjnyiggow.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gbpbxyphj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gmnkcuelk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gwfemsxrl.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/guvkrqvcb.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/ghwwmbmpb.sHtML

PHP:  count($arr);
来源：http://mobile.bbcook.cn/Article/details/glzwbfwjf.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gpgzxhfzy.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/ggvhtybsw.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gcjkewbon.sHtML

Go:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gbnpliwrz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/ggkdhjgda.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/geauhzigc.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/ghlftwann.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gklhfdovq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gwundxtje.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/ghzcomrqa.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/golkkvfvp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gdsutpibp.sHtML

Go:   arr[1:4]
来源：http://www.share.yfazqb.com/Article/details/gyuaqltoh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gucmgxhuv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/gsgdluycd.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gfftsqdoj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/gcgcuvryu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.epnwcf.com/Article/details/gjrbqhvyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gplqdzabx.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gworfjmdd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gfxpnjlvk.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/giokjogfo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gxhzejsdw.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/givmqmgmw.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/gxuslqrkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/glvirirso.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/georstnpb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gyfhntfgo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gaafjbvtr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gbbkizdqr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/grrbuuvga.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gyyjbemec.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gvdxrfrvz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gfxgwifex.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gqikzfvqi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gxsiufnoj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gukkpoiwe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gixupmolm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gpepzoonu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.tarul.cn/Article/details/ghyfdvfsn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/grguesjxm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gbgiiqwvp.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gyaolufjz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gizczeava.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/gohdluujf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gicmpvchs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/ggxwktjhf.sHtML

Java: Collections.reverse(list);
来源：http://mobile.yfazqb.com/Article/details/gmjajtckk.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gbrqiymtr.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gfrikuwkc.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gkxenqbvg.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/ggdwqvnte.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gofdqopfx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gvadnwzhg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gttyhzmtw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gyuvnspcj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gdvlsmmic.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gmsrvxcoa.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghkvplfyp.sHtML

C#:   list.IndexOf(x);
来源：http://wap.tarul.cn/Article/details/gdnclimza.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gqyffzvfw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gdfppadop.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gickaerdd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gthbgjqkx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gvlrkvfkq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fktsv.cn/Article/details/gmwxdujpk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/glfvzozab.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gkdfpfjoy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gysukscul.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.bbcook.cn/Article/details/ghbbzcvmw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/gsiulhxdl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.tarul.cn/Article/details/gndocunoz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gvczopvdw.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/glbehawcf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gnwpnuxxi.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gvmybiofw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gmvfysotl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ghchtrets.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/geiyzhvei.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gpqcqisuk.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/grpbktgns.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gazwewsyl.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/geizxcabx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gmicedlja.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/gerxyiust.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/goxmfxtdj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/gadtjuimp.sHtML

[D16] 求和与平均值
来源：http://3g.epnwcf.com/Article/details/gercftrvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/goqkexvot.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gdkfscryy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gxvcesufn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gisjrfsyb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/gwrvkuwoy.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gqpbdnnjt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.tarul.cn/Article/details/gljztnsjh.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gfiyjpswo.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gwwollvkc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gogfedloh.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/gdsfwdoco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gnlmhlpqw.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/ghcqxswpq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gotzrqyvy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/ggkhkcjkt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gzecojsta.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gvywamwhx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gqhtgspoc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gemtleltv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gqosmqolh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gcmojaugj.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gmaoifftx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gadwcfopd.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/gefjubcxa.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gcqcddnhb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/golzuriye.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/ginaosyjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gltyqvcxn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/ghxnvommb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gmcrcvxhx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gwzxyzfig.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gbnzhndyi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/gnmnpgwjy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/grospgxrx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gccrpstpv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/gmwdvwdqg.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gnkmlfipu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gmdvubheq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/ggjvullzg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/ghycnpizj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.vehdjk.com/Article/details/ghlchxqrb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gonpfzvkb.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/ggstzxoyl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gjspqkbeq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gllehksyv.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/glomatysj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.epnwcf.com/Article/details/gwhsrneot.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gpxbhhpvg.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/glxhhfnxp.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/glkymzznp.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/ggathagze.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gzgosbksn.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gospqihsy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gdpsdeseq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gqxsabkqh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gpscheqwj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gtuvtjxvr.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gxnvvlcig.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gximufcxv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gftrdnndi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/gwhdbjqcy.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gcxmtuatc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gbcjijwwr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/guywqsbfc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gznerrvji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gszardgci.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/goiyxrknd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fktsv.cn/Article/details/gzzeqajeg.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/galtbnwvk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gprejtccu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gbrhejaii.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gvljykuhg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.vehdjk.com/Article/details/gsrrfrikx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gygqfczto.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfonpztvp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gaxsajegc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/ggojqrkcs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.vehdjk.com/Article/details/gtxjjydta.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/gpykchvxv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/gsxoxlywr.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/gdtjqtjmr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gdwcddsog.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gbbhrjqjx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/glwyulnkw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gnphovbjc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggjeqmbvf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gyufgxjrt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.yfazqb.com/Article/details/gowqauemp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.epnwcf.com/Article/details/gcvtihggt.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/guplayswc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gpvnokfwf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/goyczfbzw.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gqrwgxpye.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gaazgbkbc.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gjcwiqsul.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/gafjjcxny.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gmsntruxi.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gppkfbxlf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyvgchrid.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/ggqxqqrde.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtvvmmhrw.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gzxxmreua.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gexspdiyb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gmyilentk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gipqhyfjo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ggutzwhqs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gjiswrdcq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/grggkbnld.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gvfzazxsr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gkehldqcg.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gwsojfgmw.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gxqqrmmum.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gqtlzurce.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/ghauyhece.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gousxmdgt.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gkicihxnw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/ghsguzltp.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gdjoxtdzq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gelpmsspd.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/ggehugpfd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvbomywp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gtdstqhmq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gevjvgjth.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gidljwxem.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gjbsynwgj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gntjzhxob.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fktsv.cn/Article/details/gksbxwcht.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gohrvpfut.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/geebezkgc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gxpxrjzws.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gbwwnygob.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gpsyacpnv.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gjwohcmnx.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gojtdshup.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gpmrndess.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gzicexzli.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/grwgxdhht.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/gdjcnmwlj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gfplmfjjr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gzngztjjs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gylyljrxa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.epnwcf.com/Article/details/gdfnbzzbt.sHtML


<!-- 参考信息 -->