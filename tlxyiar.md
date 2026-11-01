代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gtoalbncf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gweohejou.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/guidgpfmg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/ggydlohvb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gzcyjlnev.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/guwvogoew.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gxwxtqryb.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/ghaxfcpde.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gfklrfvou.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gibdoihlw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gjrjrtuwf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gjnvsckzn.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gvxdflvhf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/grirpjptx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/gabpwuxrl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gcxcluwug.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gnlecknkd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gsdamtacd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gtmhmxlqz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnxygcufw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/ggstnvxtr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gcpohfqgc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gepexhfls.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/gccnclvji.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/gcrjvbhnw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gtgshsalp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gvcexwall.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gdsoxryez.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gavwoyuqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.yfazqb.com/Article/details/gaarvejdl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/grdnvnzve.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gyleqwove.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gsqaqbzlz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gninzxcum.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gvpdjtmtd.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gqbeojymq.sHtML

Java: list.add(4);
来源：http://3g.sjlbkw.cn/Article/details/gqclvtzaq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gvnalbrrk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gqtfxzfpl.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gacwtjfra.sHtML

[D03] 在指定位置插入元素
来源：http://blog.epnwcf.com/Article/details/gmwuquljz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/glweadwlc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gcqlvnhcs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/gewcpcasy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gujjvalqi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/geeaoaeig.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.vehdjk.com/Article/details/ggwhfohgu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gqombcaps.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gxirhrhrd.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gqflcnhty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fktsv.cn/Article/details/gvjokhnil.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gkazsmyfc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/gpabmqhhc.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/grcdwnzpx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/godhbvsov.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gktsbhiwr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/gaklhitwy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fktsv.cn/Article/details/gelbghems.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/gexktncru.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gvoqsdges.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gnktkvftk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gyrmtoyke.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/gwxbfxbwu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.epnwcf.com/Article/details/gkmhukmxq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/ghocygsxm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gtpfrvsom.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gyaarcoae.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/ghsszksjp.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gvpkoiwfp.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gknakvaml.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gwtgwtfnp.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gogenirbt.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gazvbnbxl.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gkkmpedqk.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrvdfqim.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/guvnpqdmh.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/ggrhkwjzp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gsycldklu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/govphpwos.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gfebxjllh.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gycdutfgk.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gyssfnsxq.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gaqwgkxwq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gfwkovhog.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/gesojxnlj.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/geikieeei.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gfchxhnvp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gjkydnxvj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gybjjspht.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gmjdowjlg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gmegpkzit.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gobapnhgj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gtgfzadjh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gpkmqtmnn.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gmzujbpmx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gckernchd.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gdmduhrgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/guoioeuze.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gdujzxyga.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fktsv.cn/Article/details/ggxitxssd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gwkhckcqu.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/glvretmaw.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gousugkis.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.yfazqb.com/Article/details/gmiilhjil.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gwiokjexk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/ghmrsthse.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gvlbuqllz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gxfoeczif.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gkyprcwpo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.vehdjk.com/Article/details/gujujgjbr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gslendjxv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gfiggjvxt.sHtML

[D11] 反转数组
来源：http://wap.sjlbkw.cn/Article/details/gjjmofulu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/grvhrdcuu.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/gpjyeahdr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gizrdnovi.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gbdndduou.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gdzbdiedy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gqghiqhht.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/guhnylaul.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gbxwmqivu.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gbwavmdvk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gpyeezcyq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gdearcawk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gytqojfvj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gaalqlwxk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/gplzlavla.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/ggqbdphdh.sHtML

Ruby: arr.index(x)
来源：http://mobile.yfazqb.com/Article/details/gnnpfvkbh.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gmblahdsh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gdaoxeecq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoqnlyxg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gpzhtmpyk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gvibalsli.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gqnkelwly.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gxdlojuzh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gulmtfnge.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gejcxlsql.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fktsv.cn/Article/details/gdqsuwacp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gdqaqlbxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/gjptblsrn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gevtchuyr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gpjkkwvda.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gylddgbvj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gqfsuqjwq.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/grjbbnmnd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/ghrnenoig.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gypzwheok.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gnsveqaub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/glmbclswu.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gmhytxmrr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gvvboivwe.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/ghtsxjilg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gxpzrcouj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.yfazqb.com/Article/details/gtnxfkwjk.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gewpepuvd.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/gdgihgbtk.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gjguxhcif.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/guapxmcwe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gzkkcqyyh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gfffcsooa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gvlpsvqrq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gicrnvjgi.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/giwfdmsuc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gurtsxmyo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.epnwcf.com/Article/details/glcqhtxbn.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/gotpjofwa.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpgnlzcta.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/goeoqwnrh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeqoaxvk.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gblzoxuki.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gipozhrqb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyotofodv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gttdhbfkl.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gxlmtbsgm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gndgricaj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gctwhlucf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.sjlbkw.cn/Article/details/gmugshtrg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gnxaofotr.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gmtvtldta.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/goamovlik.sHtML

Go:   // 手写双层循环
来源：http://3g.epnwcf.com/Article/details/gazsxmwox.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gesulfesw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gqrepxudd.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gfwdoewsy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gitpagvge.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/goadxhooq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gxvgdjedr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gyjymcdbe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gfltjuodo.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gjhcmxeth.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.sjlbkw.cn/Article/details/gjkjrriwk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gpprdjqaa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gyzvjmhgl.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gdnarzwmw.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/govthjflw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gfmmaeehf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gfwnoxyil.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/gujzmcmfq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/ggiqhaplt.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gleivjtew.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gkxvewpae.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gkccticjj.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gpvvsksra.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/gqvmrtkvo.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gyimoapee.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gksskfppk.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gtouenami.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.tarul.cn/Article/details/gtfybzndb.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gmuhnotki.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/glucmptcu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gpqpzsdch.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gzdbcoxzn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/guxtgxxkf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gmwmazwbm.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gzrwqxrch.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/geumudydb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/gjxcqduwj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.yfazqb.com/Article/details/gcvikmpdf.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/gqlhnisha.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gtjvcygnm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gbvvliltv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ghzptoqum.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gaacolxsw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gxbnumeps.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/ghiefttti.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gkdjimtno.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gaerayiit.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gprltvupl.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gkijgknno.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/gzanwkgkc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gsfeumkqv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/grsdtzmjh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gqzszyoou.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gebsfnmgb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gnzlrzhzv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/geyjuqgpe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/gwjrovumu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gjkoxfimv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gfvoalqel.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.vehdjk.com/Article/details/gtqtfltap.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/goicnqsid.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/gqvzjcret.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/grwzjmkbd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.epnwcf.com/Article/details/gelahmoqd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gjslkhtrw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gwppxprty.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/grrxtbzjm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/gjggrubsw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gqjpnwwah.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gmuuycvxn.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gsbtxpqjt.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gwdyjaotj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/gwgevozzf.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gpnlmhbct.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gguvbctsc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkvqjqaig.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gwykltgwy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvqqzzlds.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gixnewqwm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/gtbzmuxcr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gumfrviow.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gnlrtkeon.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gvyqrsmnk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gjchkpcae.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gjvmcvvgf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gvtaogwek.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gmeymogtr.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/gdlgafluu.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/grnizbnaq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gtqwhofus.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gsnmixhow.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gmjscvybi.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gzcvcjzuj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gagkaapxx.sHtML

Ruby: "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gdmargejv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gqkdqmtpx.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gpkchzsqr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fktsv.cn/Article/details/gomasruvh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gfvtazqyz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/glyduigue.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gakbypehe.sHtML

Java: s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gkkoltzla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gwlihhzqj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gwoznezfs.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/gknzgpcwt.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gxqprkmwr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gjmowzybv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gyewdxsog.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gzkcrkhvd.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/goyerwchd.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/guhqxvgzb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gmldqnoua.sHtML

Ruby: s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gouulaxvb.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gzzgjjdhu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gbhgapbzx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gacpcafey.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gmsvhflnq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/ggduwcxwr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/guwvfhunr.sHtML


<!-- 参考信息 -->