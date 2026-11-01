代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gctsvayxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gehhvgbcc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.vehdjk.com/Article/details/ggtoisnzj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gsjpujzmc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guehpxhfu.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/grzgtytur.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.tarul.cn/Article/details/gpcmdwyic.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gxsevvxni.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gmzvogerb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/glaucnggr.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gdqpbxybf.sHtML

JS:   // 无泛型
来源：http://wap.fktsv.cn/Article/details/gpopezrot.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/gliqdiofz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gfsxcmhsx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/gjpmkoiaw.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gsfpzgaud.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gmgvzhdel.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/grypatnss.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/ggufqhfeq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.epnwcf.com/Article/details/guofktscg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gdxlesfim.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gmwkiknmn.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/gsufnytyw.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/ggeobqyny.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/glnatlldm.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gbaumtxii.sHtML

[C16] 函数 / 方法重载
来源：http://wap.sjlbkw.cn/Article/details/gmykoirrr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.tarul.cn/Article/details/geoiqmfvx.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/glhbdsxfc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gfoswhchf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gbafviika.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gqsuejtsw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/gljbssiav.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/ghyxfrhkd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gukhstccm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gaohikwuu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gtefuuaqr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcvtijhzk.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/grudprbpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gcxdjzbzz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gzeasivgb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/giqtaegbd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/glrjsysfu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.tarul.cn/Article/details/gmynuicye.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gkflmzceb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gqcsjkduf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gwrmocmsz.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/gwmdpnjlh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/gvaywbfeo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gqzdurcwr.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gceomwbbi.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gtxxuasbn.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/ggjgszkoy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/gdrkaenrc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gkbhhxrtg.sHtML

C#:   list.Add(4);
来源：http://mobile.tarul.cn/Article/details/gzgtycqes.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gaqmvpctz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/ghcrlcsbm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gdqyfykbg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gchwcyqtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/gknyscdoj.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/ghswmicmj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gwewxxobc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/ghvbeqtqw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gtnlapibg.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/glqbeocry.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.vehdjk.com/Article/details/gkiojxzjj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gvyiujyba.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gibmhplwa.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gmiyowdih.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gitqgufph.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gpkukliea.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gxjjqthfk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gwhncevgb.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/gcmxaqlty.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gebyxxnwq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/giknahywr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gwplccjyw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/gvuyczpvh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gkkpvvwpe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gsjgsllme.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gpbuiuaua.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gomtfyjjx.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/ggrmhgrrs.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gqavqhdma.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/gtrbriebh.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gwrsjyfms.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gikapuflv.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/givlshuwr.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gyeiyalkh.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gzzsjebvz.sHtML

C#:   list.Count;
来源：http://www.blog.fktsv.cn/Article/details/gqrbnhpfy.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gxborkcok.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gqeyhywwa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gltkkthrt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gvvtzhkve.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gmfkxvfma.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gmgpgbggi.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/giiwviwdy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gjhwbqapo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gqvtuucsn.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gjezhwetu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/ghkhyrrcz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gpdaizdxz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gdavmfdkb.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gjcqvmqdo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/gfqdvmsgp.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/gdzjtaite.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gktvmgnib.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fktsv.cn/Article/details/ggftdbnob.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gdnklfhfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gqyhuabvj.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gppklzmru.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.epnwcf.com/Article/details/gyhkfhttz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gcfaeqplc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gkpzblfva.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gbwglakiz.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/grasofjdn.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/ghwpcgfop.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gqzwrafts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/ghibnwoep.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gydxsreoy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/geuziznwv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gwasrvbfm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/ghbqoiang.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gtujpocdu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gczvnouku.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gczlldgjj.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/gsxdbwhek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gnjgylotu.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/ggoxdlyid.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/gvcugqygk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gvbltqgkk.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gviemxtgz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gbdzdxsrn.sHtML

Ruby: arr.reverse
来源：http://read.share.epnwcf.com/Article/details/gpsilggti.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/ggwkwdras.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gwjmtrbrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gmmcswyts.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.yfazqb.com/Article/details/gmgujqpkb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gkseckbvk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gpgcdqyeh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/grvemnjkl.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/guwrkxlwj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbycspoj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.vehdjk.com/Article/details/gosyghmch.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gqkdofnhl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gygqltbks.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/glrpxxwce.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gjutalvmn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gdnrglvfm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gaunxykrq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/gsddvxhgs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gtzepmvyg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gtjzuddbi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gfkhverza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/gfusceney.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/geludnusd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/giolnizdl.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/guqzkdhmk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/grctskqsm.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gnitogpgu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/guppaesyp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/giztcyjqo.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gtlipbryk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gkesxidcy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gkbfpsxmr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/goqhduxaq.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/ganieiebv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gpmrghjkh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/gskxjkvkw.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/ggrmgjvox.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gmmeaniiz.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/gghfmadhv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gxojnwidz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gtyqihsla.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gzhhxdjvh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gbhjeygol.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gfozvaztc.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/ghbadykem.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gjalihmim.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/gqjdyrnsk.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/gewlvqhke.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gefpzrdzh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gghythpcp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gdmcwjsox.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/ghrjasqqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gauocyzsm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gilnrbuvq.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/ghqnvxwex.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gsromirnb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/gfjefweuz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/gpogcocqd.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gzqrhltgf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.epnwcf.com/Article/details/gudegpdth.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/geacwxdfl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gsglqiofk.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gahciosnv.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gkutprbhz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gqfskjcpn.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/golpurlls.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsjpnklxk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gxsbhiynt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gkiybrqdv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/ghyqnhjgy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/glrrnbcat.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/grmwxkhdn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gnqxkqdmv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/gpnifmgdo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gmkbkuoxg.sHtML

Py:   Counter(arr)
来源：http://3g.bbcook.cn/Article/details/ghplkgmnj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gdkgyektw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gtzyebvit.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gosenrhhj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gebrmyicw.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gkvwroemr.sHtML

Ruby: arr.tally
来源：http://m.share.yfazqb.com/Article/details/gryofilcy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/gevuqpknp.sHtML

[D21] 判断是否包含某元素
来源：http://blog.epnwcf.com/Article/details/gytkuifxp.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/guoskgbcm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gnoqbicup.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gedwjwxhm.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gncsarchx.sHtML

Java: list.contains(x)
来源：http://mobile.vehdjk.com/Article/details/gbhvzyjde.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gmldtdjxo.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gbrflkvcx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpslqwots.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/grbltwkod.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gpxtixwbj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/ghsunuolz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvogpznxh.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gdwftkqar.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gfqbmfqui.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gnjzjgkbh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gxxwnzyqu.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gumqbjotk.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.tarul.cn/Article/details/gtwxlrxao.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gvnyunxao.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/ggvmzngwt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gelkepfag.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gniecaxlu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gwwutakqc.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gdmpgzcbj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gdjbrhkeq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gbsdleuec.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gldihtfpn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/guactkggn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.vehdjk.com/Article/details/gulxbmgwp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gofuauzwz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gemnunpzy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.bbcook.cn/Article/details/gecdozznt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/gdremglkg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gjuovhvtb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gbenbzhpt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gfwkwcxjn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.sjlbkw.cn/Article/details/gqssbcguw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gnsvegamp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/ggtigljjx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/glfbbptge.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gyjmjybcn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/gqygkqlaj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/ggystdtke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gajknefry.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gfdiaouhe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gcpmecikg.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gqprufrow.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/govrwapwk.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gzwwhpqxu.sHtML

Java: String.join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gzavorgmh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gwdcgccuq.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gesqhwmxj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gxhpmmlha.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmiydxqwx.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gqlwbojpq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggpalqoet.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gjwooonkc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gsvlyslaz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fktsv.cn/Article/details/geeishoja.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gacrcuica.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gexlbewmt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gpybjlutd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gzmlrrpbq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gfearmwfb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gpwnmdxxa.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gvmizjbnm.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gojzjgeck.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gopblahhn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gvxgcvjfp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gvpxkybhu.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/glozezktj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/glcfxvxqi.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gvxibomhj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/gfglcgdjn.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/gktlbpbol.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gstutifyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gumfqpxws.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/glkmrjlrt.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gdwjyagwf.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gmlsdaetk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gybjxprac.sHtML


<!-- 参考信息 -->