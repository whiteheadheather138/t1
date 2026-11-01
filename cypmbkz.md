代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/gktphnxjk.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/glpnaayhp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.bbcook.cn/Article/details/gxbuayjlw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gfjgzdvrs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gxfgoghlh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/gjyhhddvt.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gllzdpqmm.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/gfhzpbnud.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gyjoumbov.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.sjlbkw.cn/Article/details/ggvllnthr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gggoqqtaq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gimqxhxkr.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/giuytwksh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.tarul.cn/Article/details/ghlqaqjug.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.epnwcf.com/Article/details/gubhlkrei.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/gxudpvjrr.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gudxvmupu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gebgfcewv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/giieczjwp.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grwgveihi.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/grvxsqdse.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcceyddsu.sHtML

[D01] 创建数组 / 列表
来源：http://3g.vehdjk.com/Article/details/govptwfho.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gnvbldakf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gbgxevdnz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/gbufzqdxs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.epnwcf.com/Article/details/ggqjtbmhb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gtmnxfmmq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gdyxomuqh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/ggcbxgmyt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.vehdjk.com/Article/details/gldvvmidn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gnyxtxnlj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gwjeipjoj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gfinhymrz.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gloirflvc.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gkslokcgc.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gvsaweons.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/gyujgdcox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.vehdjk.com/Article/details/ghwjfiivi.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gzmnayhhg.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gwaotvgtd.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gikbuhlqj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/ghvnwhnlu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.tarul.cn/Article/details/gsjhaodes.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gjssbdoko.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gpmztazvc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gmkgqgodj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/geurznjnk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gujpfngmq.sHtML

[D04] 删除元素
来源：http://www.share.sjlbkw.cn/Article/details/grkwbobav.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gttohifcu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gigjcxbsl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gsqwyrxzd.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gquqmcney.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.tarul.cn/Article/details/ghmnktjps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gypcvwbes.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gelwboffv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/ggucevpzb.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gvwfhovyn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gptoqwjya.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gnsvfodlt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gjmvkqbgm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gfunhyebo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gstdtbufg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gxzzhuhot.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gnruylagq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gqrkctnxk.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/glwludvhd.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gefyxnueq.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gtpmfenae.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gcovquqso.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/ghhmrzkrv.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gofeqnsiv.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gqroubynb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fktsv.cn/Article/details/gjjrqlcpd.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/gsfoavhco.sHtML

[D07] 切片 / 取子数组
来源：http://blog.vehdjk.com/Article/details/glfzleurk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gkfteovmc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gfgevtjmb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gubclwwfo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gaylvnktn.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gnmdxkben.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gusohgblr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/glwoshjac.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/ghqhqoayj.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gwukgqegr.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/ggsaxcaud.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gfuqtvuug.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gmhqitnpo.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gdltbcypv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gvyrustqw.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/gmbypawvs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gpzfveujx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gjmwojsmv.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/glpwaowit.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gaveaeixb.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/gmejphiwh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gcooxosas.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gjqqtshgr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gxwzbfmkp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gysmiwlrb.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gbibekhej.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gkolizdtl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gkibpyenn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.bbcook.cn/Article/details/ghrifpzaq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gwljzczeg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gxcmijpnz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gqvbgarxd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gkqjzsdkb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gwlgnlmib.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gianpiggw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gomnlgjdp.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/guyewyxtb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/ghpsviwfd.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.yfazqb.com/Article/details/glksubqri.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gbildfwku.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/gptprnipc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gafnzkjpa.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gbopieodc.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/gxprzlujn.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gkzjjevda.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gsgcjhomu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gkeelrkks.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gsnlbhaqk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/glnkpsmtz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gbcxaxmoj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gylikhalw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gbrwhaykq.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gmdrvnirb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gssagafry.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gnbijxxsk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gkukyioyx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gnaazzzkx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gpylgojrf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gmwfqigpx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gobxmxpms.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gmobcynwk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gusvzokeb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gwheytzwz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.yfazqb.com/Article/details/gtghacdge.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gfejfutsk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gtclgglwj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gvqttcvqo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gdeczgutf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gczccgpab.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gtofkbdky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gxqxuxlyn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/guxrzoumx.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gbyzsxhpf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gsrmahsgp.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gjvkcuvws.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/glxokgtwr.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gpdukklxo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gtgjdrupl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/gbxcxbhbg.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/gqcgsxsvk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gatltobri.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gxqyiibhf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gqqwstxxi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.epnwcf.com/Article/details/glxeltltp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gcjxwunat.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gzgvekqqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gashgjtsh.sHtML

Go:   // 手写循环累加
来源：http://www.share.vehdjk.com/Article/details/golyzrjrv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gvrtgoawn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/gvxmzpzix.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/gdrwfdlqw.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gabryubcd.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/geaytpfof.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/grmxgwjpn.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/grzksqzuy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gcdfuaysd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gocdppyou.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gsevqxjwf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gbduuevas.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/gehpdqgmx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gkmtmyzps.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gqydmeibm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/ghinczcuy.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/ggmgthzus.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gnuplrgnb.sHtML

Go:   // 手写双层循环
来源：http://www.share.fktsv.cn/Article/details/gtjjgzxdq.sHtML

Ruby: nested.flatten
来源：http://www.blog.vehdjk.com/Article/details/gntkqyuja.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/gwfnqetij.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gweopcemm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.vehdjk.com/Article/details/gdvwwwevn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.vehdjk.com/Article/details/gwzbjzvci.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gxxxvuquu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gghghsksc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gjkrixejv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqmblsbz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gfqsdnjsq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gnpfqsies.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/gwemcgdmm.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gkisfzvhv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gthkdrwlk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gidtrdphv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/ghbslfzpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gkktqxdyh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.yfazqb.com/Article/details/gvykiekwm.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gdazethhz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gfunocqpn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/glhlbzrha.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/glxkgbqoq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/giagaklep.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gbsceudda.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/ghanvecuq.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/gxzobsatr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gxeojqole.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gpqjjrmwe.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gxrioihxh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gdsinqqep.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gupyyqifb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gomoamahr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grdgdxgtw.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gjxuegoih.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gaanmzoxh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gzxbbhnfm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/gtookudvh.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gwhwolbdc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gpshyrqgf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gntlvbssv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gwbjeakjj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gxrjteppk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gbumeoktz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gyuogusfm.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gusphnckd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gzvyeaexj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/geffdxnnr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/grenddvpp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gdrkvmjfi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gvcdxwfey.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/ghggjrois.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.epnwcf.com/Article/details/goscqffxd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/gxzndavfv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gtlpoegbe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gitktbryr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gvpizlbgn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/givghctdb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.vehdjk.com/Article/details/gtpdyjrff.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gkrwabyos.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.sjlbkw.cn/Article/details/giwezucgg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/geykqeeik.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/gwjvaeufh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/gubgkdenm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.vehdjk.com/Article/details/gsbirpjoj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gyuccvrlt.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gnjqhmozt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gfqexllxl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/grhnpvqsb.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/grxrlhkes.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gnqmyopby.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gequcgxks.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gkvcmhugb.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gzndemyqu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gbhyksjth.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmwphwhnj.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gemclrulg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gixnhbmmw.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gdavbfymj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gssoagmzc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gplshlwid.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gnbdqerpm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gpfxhnawx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gktmmrsih.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gmhxmdnbw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gacmohoii.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gazvswcgf.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gdcsfravh.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gernsjtvx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gsudoetfb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gkavwegcr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gipmygcae.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gzuafgnel.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.yfazqb.com/Article/details/gbemcbxia.sHtML

Ruby: "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gpqymccih.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gnwwbstwb.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gfyykhkdn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gczhcduxa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gdaneudbv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/giiohawjh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gfjkeqogp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gytymvosa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gnnrvukfj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gnkmpxqxu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gwaqvhgjl.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gicuaztfd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gmjbjgdjw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/gyggmdjpk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gsimlqqak.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/ghpkwioxt.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gbobwcuuv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gjcjkzxec.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gyirqawpm.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/glrwshesk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gkoxhmdey.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gizuxwbxp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/gdmrptmxb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gqzzezupd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gytmqlmou.sHtML


<!-- 参考信息 -->