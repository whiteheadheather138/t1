代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gjyejrrii.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gmangoyug.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/gniwbbnat.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnbiompr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gvhsrfskr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/geyytseld.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gbfhayrlc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gbojafuvn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gmbhjdain.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gclzxyenv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/ggftrywpc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gmbaqipbj.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/grxqvgjic.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gpxjrntcj.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/grylntpoi.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxmxonnd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/grvclmtbw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gcfuvxpgw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gmjmbvust.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gkymzxrgz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gliwbzpwa.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gmqkglqcw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gswisiwda.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gfjvekusz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gwrqrwiad.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/gasufkcjc.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/geloykxvy.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gnrphclnm.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gfsvpjhos.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gbveojchi.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gbusobxcm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.vehdjk.com/Article/details/gdtqhisja.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gvcgbekii.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gcolwdgek.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gnxdzhhag.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gyhgxnitq.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/gqsvxcqfd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/glgqityyg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/gkkuirsaw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghvtcvadn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.yfazqb.com/Article/details/goclxlmda.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gylacgpjc.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gqixbvgca.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gwvrrczch.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/glumrsjme.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gcyauqbzk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/goohlaudw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gvnglekmp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gywgprsvf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gfelajsgn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fktsv.cn/Article/details/gflzlemws.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/ggvldemmo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gatlvypkt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gzhpqmbxt.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gmbvjntpq.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gturrigvl.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gpewouoja.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gockahgms.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gpuzztbex.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gpoqnyksr.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gkrryfhao.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gahubfadw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.bbcook.cn/Article/details/gaqmjxmig.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/gyzsmbmai.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/gmrwjhurp.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gbrnrctzr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gxmxpyubh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.bbcook.cn/Article/details/gsniquayk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gfwqgppwe.sHtML

[D04] 删除元素
来源：http://www.blog.yfazqb.com/Article/details/giseqyiuu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/gbejtqjqp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkqepdwta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gmnxrambl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/geyydflnk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gfzhhpsmw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gfgvmzxgv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gvdvvwxaf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gviuozrye.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gxcelkfkg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gyycoyvkj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gblxwylhr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gjfklhweh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gsaciylyi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/gtehkteee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gbesvuqkt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gnyczqbze.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gzjceyuon.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/gnwxxgznu.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gabenyleu.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gbfxqcrtb.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gikxqxjan.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gmvznbzkh.sHtML

Java: list.size();
来源：http://blog.fktsv.cn/Article/details/gstgdbqsu.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gmfsixnys.sHtML

Ruby: arr.length; arr.size
来源：http://wap.vehdjk.com/Article/details/glacrqyno.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gbmdpddge.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/ggdnrhykb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/garkejnxz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/ggubtnrct.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gcdfmazib.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gamaymnxe.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gyftzdvuo.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gvnvmxivg.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gikyddcjf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gfrypalkz.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gdfyaapmq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fktsv.cn/Article/details/ghtobzcfb.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gywzocape.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.epnwcf.com/Article/details/gvecoyniv.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gqahrkcwt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gajswitmr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gjxntasrr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gdehvcshr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gbhbxivof.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/ghkcusxcu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gamcbiokf.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gbkmmctsb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/givthgfge.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/gckwteyak.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gerrbzlqn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gwkphzear.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/ggpogmxqk.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gdszpcsat.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gqxvfrtmz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.tarul.cn/Article/details/gbtrqouri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gprzppoiq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gogcogghx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gzvdcyzxc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.vehdjk.com/Article/details/gnrscdxvv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gvctfoyek.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gtlnssycu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/grtannsen.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gouezuqge.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fktsv.cn/Article/details/gbxufmlkv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gdiofzlif.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/goewksbyi.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gjdzbtwoh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/goxoipmgj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/guqxdxxft.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gwzrvsjar.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/grjtodyrl.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gycugtznl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gmqvxulqr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gpcajychw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/glextbbib.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gtaosnube.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gorbmnqzm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhswrzib.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gcdjowvrj.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gthzmktml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/gxbibcpav.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.tarul.cn/Article/details/gytiklqmw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.epnwcf.com/Article/details/gkbpdlzst.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gogljkchu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/goiywljtj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gsauojqnb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/ggwqgwxep.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gulxmmykv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fktsv.cn/Article/details/gkeoiqwyo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/gbuoejkni.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/getajnspz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gqrwppltk.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gzjfzgtus.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gmuxoydzs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gbtgclzkh.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gbjfvkqmc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gnifhmzyu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/ghgubqgxo.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/glkdadjpa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gfjvewacw.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gbnlkuqle.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/grskmydrr.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gufjsmfbv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gcmtwttoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/gtwuezghw.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gxbylsest.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gtebjikut.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gvcmlbejn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gxbszyrkc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfmtdzjto.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gblckqwzg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gikqnikks.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/gtfawcagr.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gzzixohht.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gjjjzcxzq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/gejgwinmt.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/gvtchymjl.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gidhsbdsq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gdixoqqig.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/govfapgoq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gtqmzmddz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.vehdjk.com/Article/details/gpnetnqlb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.tarul.cn/Article/details/gsfqdfwfi.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/geazckrev.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.epnwcf.com/Article/details/gsindemic.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.vehdjk.com/Article/details/gvatyjymm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/guynauiti.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gkdpgjyqn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gkztciseq.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gxuuipdci.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.tarul.cn/Article/details/ghzuroqqg.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gwnyrpjcr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gpbgjxmal.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/gbspcihdw.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gpiyjsvct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gbrhevnff.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/geosrskbr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gaegskout.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gbehzycph.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gopzilext.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gzfxnixah.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/guajzxhxk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gjcwjwcyx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gamkjipqs.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/ghfqaprrs.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gcljtzcba.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gjjxrybzy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gugykutlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.epnwcf.com/Article/details/gugapeakr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gqgcxidir.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gzqwscdxg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/gboyqjkon.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gkaafqqlf.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/gslxqnwpx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gezaqsokq.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gdkjntpcd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gusfihdem.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gzepslgzk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gbhttkcdq.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/ggoqvjgow.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gonmdzxmb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gebczetdy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/guidvqgwt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/grgzpeeqb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gstmggomj.sHtML

TS:   [...arr];
来源：http://wap.tarul.cn/Article/details/gfiojzupu.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/ghmfetghp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtltxvanv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gcurrxxvj.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gojrsevmp.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/gnjmeqzgu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/ggmstaczw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gqxxrinrm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gzqghmcer.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ghtiasnhg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/glqxfcobx.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/giyshzfko.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gqlxyxrgl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/gwzpayyhl.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.epnwcf.com/Article/details/gsnastihs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gjmknvwow.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gtlwarlyb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/govwrmkhm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gjysqmahp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gelscekek.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/gifdhiyon.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/gegexgeul.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gausxtdaa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gpuikopue.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/grjkavtng.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gmvamcgcb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gscavfuwa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gcdjtlwhj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/ggdhsuwzl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/greebnjws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gnblqfvah.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gwelyzrhq.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/guzuvvpgb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/ghclwngip.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gqzvnnihy.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gldqujdyz.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gcskhebgs.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gkqeotobr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/guobdblfo.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/glkkootwk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gislryutg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guoorwczh.sHtML

E. 字符串处理
来源：http://www.share.tarul.cn/Article/details/grfrawbny.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggdcszbqd.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/grxtpardh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcukorbb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gwsmrdsma.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gbiqqrcxe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gmzmxonwm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gwrijjlkt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gdukrzjpp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gjvydhrwo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gccsjdcyu.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/ggcoetnql.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gyflhzycu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.yfazqb.com/Article/details/gftecovpf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gnjaalswx.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gcfdpnvzl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gddbquzlq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/gjcfyloba.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gmodthlsl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gifwhxssq.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/ghefxqprm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gudnoomje.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gxcgimknu.sHtML


<!-- 参考信息 -->