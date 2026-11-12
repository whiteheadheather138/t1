代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://utb.andypj.xyz

Go:   func add(a, b int) int
来源：http://ngp.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uhn.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://kve.sufxvd.cn

[C14] 泛型函数
来源：http://ojo.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ear.yj20258888.top

PHP:  // 无泛型
来源：http://kpq.dianchejie.cn

JS:   // 无泛型
来源：http://iae.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fpg.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hhm.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bzr.nwbrower.top

Ruby: # 无泛型
来源：http://vsd.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lkh.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://xop.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jqi.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://dkl.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://keu.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://psz.gogol.net.cn

Java: // 无解构
来源：http://ymg.daria6918.cn

Go:   // 无解构
来源：http://zip.wangdashe.top

Ruby: a, b = pair
来源：http://lun.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://nrq.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://pmn.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aza.jinqigfzy.top

PHP:  // 无重载
来源：http://eek.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dgt.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://vax.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oej.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://pkw.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://lwb.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xjm.smart0.xyz

================================================================================
来源：http://nge.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://xyj.tarul.cn

================================================================================
来源：http://dyh.daria6918.cn

[D01] 创建数组 / 列表
来源：http://erq.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vbg.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nhz.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wix.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mfv.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zww.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://xmg.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://noz.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mng.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://bhy.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dmg.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fzs.zdbjq.cn

JS:   arr.push(4);
来源：http://swp.guannengcc.top

TS:   arr.push(4);
来源：http://xrp.xziqi.cn

Java: list.add(4);
来源：http://trl.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://crd.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://oil.316326.xyz

C#:   list.Add(4);
来源：http://utk.cashguo.top

[D03] 在指定位置插入元素
来源：http://bif.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://kvt.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://liu.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mdr.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://zlg.gotoacloud.top

Java: list.add(0, 0);
来源：http://hgc.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rhs.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lil.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://jui.hcnkem.com

[D04] 删除元素
来源：http://mtg.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pxy.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jjk.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zvd.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://gpx.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rlb.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jeu.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://evx.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oiq.0kj1m.cn

[D05] 访问与修改元素
来源：http://lih.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://prq.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iec.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bga.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://aot.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://oji.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://vbw.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sjj.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mow.yongpay.top

[D06] 数组长度
来源：http://nub.hcnkem.com

Py:   len(arr)
来源：http://hvw.zhiwuduotai.top

PHP:  count($arr);
来源：http://qiq.wangdashe.top

JS:   arr.length
来源：http://rpq.iojbl.cn

TS:   arr.length
来源：http://nal.yfazqb.com

Java: list.size();
来源：http://ucd.nwbrower.top

Go:   len(arr)
来源：http://mpo.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://fjx.hesvh.cn

C#:   list.Count;
来源：http://ajj.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://nil.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wuy.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://mrn.tarul.cn

JS:   arr.slice(1, 4);
来源：http://dxn.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://kxf.daxiang520.top

Java: list.subList(1, 4);
来源：http://ply.hesvh.cn

Go:   arr[1:4]
来源：http://zmx.iojbl.cn

Ruby: arr[1, 3]
来源：http://raf.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://ccn.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://chz.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://jte.pycfn.com

PHP:  array_merge($a, $b);
来源：http://xvg.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ega.yj20258888.top

TS:   [...a, ...b];
来源：http://lmd.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cxm.dashuyun.cn

Go:   append(a, b...)
来源：http://mhm.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://dmw.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://xnm.jlsjyb.cn

[D09] 排序（升序）
来源：http://nve.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://wif.birdmap.top

PHP:  sort($arr);
来源：http://ogf.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kvf.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kpj.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lph.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sbm.yanxiufei.cn

Ruby: arr.sort
来源：http://hnt.nanxinkj.top

C#:   list.Sort();
来源：http://qaa.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://whb.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cez.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gch.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://djc.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ajq.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sep.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vzh.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lob.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://soz.nanxuanxn.top

[D11] 反转数组
来源：http://dzq.svipenyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lfa.sysykeji.top

PHP:  array_reverse($arr);
来源：http://fsg.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pcm.jqgfzy.top

TS:   [...arr].reverse();
来源：http://mqo.jiagoushi.top

Java: Collections.reverse(list);
来源：http://npd.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://auv.ivvv.top

Ruby: arr.reverse
来源：http://mst.sysykeji.top

C#:   list.Reverse();
来源：http://jwd.yj202588.top

[D12] 查找元素下标
来源：http://stl.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://cna.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kck.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ypj.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lmm.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hoq.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://tac.aizwys.cn

Ruby: arr.index(x)
来源：http://tub.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://ion.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://zai.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ofv.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eac.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://ios.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://jtp.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vfx.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://roe.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://rmf.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://spb.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://ltd.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ifr.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zxt.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://yhh.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://kwr.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lnv.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://tti.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://iyc.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rjq.shanyushiyangkeji.top

[D15] 去重
来源：http://fyy.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gix.bjfxy.top

PHP:  array_unique($arr);
来源：http://qmp.iojbl.cn

JS:   [...new Set(arr)]
来源：http://hjh.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://qzu.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zke.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://lob.hnqzz.top

Ruby: arr.uniq
来源：http://xre.hammf.cn

C#:   list.Distinct().ToList()
来源：http://qqn.wangdashe.top

[D16] 求和与平均值
来源：http://iil.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hrw.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ccv.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hoq.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kkf.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wpl.tian-w.cn

Go:   // 手写循环累加
来源：http://lvu.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jbb.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://zya.cashguo.top

[D17] 最大值与最小值
来源：http://twm.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://dky.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://haw.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nfc.svipenyu.cn

TS:   Math.max(...arr);
来源：http://que.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://okq.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dbd.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://oif.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://rmw.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://gia.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://shx.cashguo.top

PHP:  array_merge(...$nested);
来源：http://yxy.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pwi.hongshengwenyu.top

TS:   nested.flat();
来源：http://xlm.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rok.ctjpmb.com

Go:   // 手写双层循环
来源：http://zns.redwolf501.top

Ruby: nested.flatten
来源：http://jbs.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cll.9152youxi.cn

[D19] 按字段分组
来源：http://uwu.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ray.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://phb.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rog.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rcm.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bcg.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://wdy.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rrn.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ftk.sweek.top

[D20] 统计每个元素出现次数
来源：http://uqa.daxiang520.top

Py:   Counter(arr)
来源：http://ypv.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://bzl.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://peu.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cio.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tbq.gzhubu.top

Go:   // 手写 map[T]int
来源：http://cxx.xziqi.cn

Ruby: arr.tally
来源：http://isk.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kqb.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://ssi.hysaishi.cn

Py:   x in arr
来源：http://dvv.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://cte.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://vlw.yanxiufei.cn

TS:   arr.includes(x)
来源：http://hgi.svipenyu.cn

Java: list.contains(x)
来源：http://mco.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://pcr.shuidangran.top

Ruby: arr.include?(x)
来源：http://vhp.gzhubu.top

C#:   list.Contains(x)
来源：http://msz.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://frl.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lkw.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://afi.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://goy.tarul.cn

TS:   [...arr];
来源：http://hdq.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://wdf.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://sno.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://pvn.yanxiufei.cn

C#:   new List<int>(list);
来源：http://cfq.gotoacloud.top

[D23] reduce 累积计算
来源：http://mcc.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pcr.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qdv.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qji.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blq.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://arc.cdnleiting.top

Go:   // 手写循环
来源：http://kba.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xyz.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zne.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://plj.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lxn.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://otj.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://krr.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ynh.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xve.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qmw.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://euz.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nyu.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://odk.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://icq.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xdz.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://usd.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jgw.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txs.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ymj.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mbm.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xtn.feifeiyinyue.top

[D26] 数组转字符串
来源：http://fnw.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://lmg.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://vkj.tian-w.cn

JS:   arr.join(", ")
来源：http://lhw.svipenyu.cn

TS:   arr.join(", ")
来源：http://axo.hfpthk.cn

Java: String.join(", ", list)
来源：http://mtf.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://hcg.cdnleiting.top

Ruby: arr.join(", ")
来源：http://vfw.cashguo.top

C#:   string.Join(", ", list)
来源：http://pqp.zdbjq.cn

================================================================================
来源：http://owh.ydjk.org.cn

E. 字符串处理
来源：http://mev.nanxinkj.top

================================================================================
来源：http://etw.chenlongwang.top

[E01] 拼接字符串
来源：http://hmj.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vuz.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://awu.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hvb.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnk.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mea.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ftj.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wfs.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://efd.zhixingplan.top

[E02] 重复字符串
来源：http://tsj.jinqigfzy.top

Py:   "ab" * 3
来源：http://apm.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://hth.sweek.top

JS:   "ab".repeat(3)
来源：http://vcn.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://jpx.yuxming.cn

Java: "ab".repeat(3)
来源：http://drb.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://iki.vehdjk.com

Ruby: "ab" * 3
来源：http://vsw.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oyk.redwolf501.top

[E03] 截取子串
来源：http://enn.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yzh.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dju.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lgv.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://fzb.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://jnx.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oxh.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://twf.uphjek.com

C#:   s.Substring(1, 3)
来源：http://vcn.9152youxi.cn

[E04] 查找子串位置
来源：http://oci.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://zja.tarul.cn


<!-- 参考信息 -->