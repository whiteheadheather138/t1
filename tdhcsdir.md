代发 wailian999

[C14] 泛型函数
来源：http://ras.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ytm.ybcxt.top

PHP:  // 无泛型
来源：http://pah.wangshuangyany.cn

JS:   // 无泛型
来源：http://aio.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://swu.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://evy.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pvr.0kj1m.cn

Ruby: # 无泛型
来源：http://muv.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xfu.mhx1999.top

[C15] 解构 / 展开参数
来源：http://isi.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bis.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://wor.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yqf.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://usk.ydzc1.top

Java: // 无解构
来源：http://zue.nwbrower.top

Go:   // 无解构
来源：http://gel.tianlin.xyz

Ruby: a, b = pair
来源：http://ked.havefunace.top

C#:   var (a, b) = pair;
来源：http://iht.aizwys.cn

[C16] 函数 / 方法重载
来源：http://wad.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xhs.daria6918.cn

PHP:  // 无重载
来源：http://ove.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nta.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://stk.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jzq.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://rmy.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://bip.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://msd.vehdjk.com

================================================================================
来源：http://ilb.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://efb.guowangkeji.top

================================================================================
来源：http://rgx.sxryk.cn

[D01] 创建数组 / 列表
来源：http://upf.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://who.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kbi.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gtt.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nsa.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wxi.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://glk.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://uig.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bsj.ydzc1.top

[D02] 追加元素到末尾
来源：http://dhk.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jdd.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zjg.bjfxy.top

JS:   arr.push(4);
来源：http://fgs.zhijiandao.cn

TS:   arr.push(4);
来源：http://fik.tianlin.xyz

Java: list.add(4);
来源：http://wfo.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://geh.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://pnv.fktsv.cn

C#:   list.Add(4);
来源：http://eoo.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://bqo.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://oim.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wrv.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bgr.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://oik.hywenlv.cn

Java: list.add(0, 0);
来源：http://jeu.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://lab.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hnp.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://igo.sxryk.cn

[D04] 删除元素
来源：http://fiq.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://haa.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmd.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://isp.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://reb.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lcf.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lrv.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iyu.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mee.xuanzx.com

[D05] 访问与修改元素
来源：http://gli.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gle.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yjg.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mqb.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://dlv.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://eox.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://okj.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hll.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dsn.wangdashe.top

[D06] 数组长度
来源：http://fhg.tianlin.xyz

Py:   len(arr)
来源：http://kki.mhx1999.top

PHP:  count($arr);
来源：http://iiy.tarul.cn

JS:   arr.length
来源：http://oem.zhijiandao.cn

TS:   arr.length
来源：http://tng.hnqzz.top

Java: list.size();
来源：http://xzf.gaohongyu789.top

Go:   len(arr)
来源：http://wii.cheryme.top

Ruby: arr.length; arr.size
来源：http://eqv.dashuyun.cn

C#:   list.Count;
来源：http://nqs.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://bkb.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uhj.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://oei.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://mvn.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://tqf.yvedp.cn

Java: list.subList(1, 4);
来源：http://lct.cucudq.cn

Go:   arr[1:4]
来源：http://ded.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://shb.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://rfx.zhixingplan.top

[D08] 合并两个数组
来源：http://jtn.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://yaz.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://szm.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wrh.jqgufenzy.top

TS:   [...a, ...b];
来源：http://osv.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sda.cashguo.top

Go:   append(a, b...)
来源：http://nut.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://cig.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://wwg.iojbl.cn

[D09] 排序（升序）
来源：http://jhl.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://oeq.zhiwuduotai.top

PHP:  sort($arr);
来源：http://yas.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rdj.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pux.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://von.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rlj.fzhhl.top

Ruby: arr.sort
来源：http://tuf.ppjwa.cn

C#:   list.Sort();
来源：http://nbh.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oob.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vuu.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oen.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aql.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zbo.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ckr.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://chu.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ghc.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ozh.jlsjyb.cn

[D11] 反转数组
来源：http://deh.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ojs.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://cnr.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kwz.ehwqpu.com

TS:   [...arr].reverse();
来源：http://tgj.yueranfly.top

Java: Collections.reverse(list);
来源：http://lds.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://oju.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://sdr.yueranfly.top

C#:   list.Reverse();
来源：http://jjg.hnxiangtu.top

[D12] 查找元素下标
来源：http://juu.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://hns.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oij.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zad.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hju.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://has.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://sml.ydjk.org.cn

Ruby: arr.index(x)
来源：http://vta.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://pfx.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://fxt.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tdp.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://skl.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://umu.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://kvu.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ojx.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uki.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://gnn.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lba.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://pkc.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://prr.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uxt.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://dvl.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://chw.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tck.jinghuilouyu.cn

Go:   // 手写循环
来源：http://ywa.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iws.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ejg.redwolf501.top

[D15] 去重
来源：http://tdi.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ubn.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://xfn.yuxming.cn

JS:   [...new Set(arr)]
来源：http://nvt.tarul.cn

TS:   [...new Set(arr)]
来源：http://qst.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jxi.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://eeh.hcnkem.com

Ruby: arr.uniq
来源：http://crs.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://wqw.yonumen.top

[D16] 求和与平均值
来源：http://goj.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lhh.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xce.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ljq.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://utv.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uww.gogol.net.cn

Go:   // 手写循环累加
来源：http://olu.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://maz.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://fea.yonumen.top

[D17] 最大值与最小值
来源：http://nxw.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://bxb.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://zqh.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gft.yueranfly.top

TS:   Math.max(...arr);
来源：http://tjv.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zna.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://trx.cheryme.top

Ruby: arr.max;  arr.min
来源：http://goz.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://jyi.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://rpb.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xhj.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://hnx.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yne.zhongyouzk.top

TS:   nested.flat();
来源：http://clz.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://njx.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://dum.fehbvm.com

Ruby: nested.flatten
来源：http://knv.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tex.nwbrower.top

[D19] 按字段分组
来源：http://bgp.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xml.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://khy.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ips.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ruw.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vla.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://lnf.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ffe.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rcd.uphjek.com

[D20] 统计每个元素出现次数
来源：http://vil.hysaishi.cn

Py:   Counter(arr)
来源：http://urb.epnwcf.com

PHP:  array_count_values($arr);
来源：http://qcr.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lsh.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vcz.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hjb.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://ybj.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://meq.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fpr.xinyue.icu

[D21] 判断是否包含某元素
来源：http://ycf.hysaishi.cn

Py:   x in arr
来源：http://lyp.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://dic.nanxuanxn.top

JS:   arr.includes(x)
来源：http://vbc.uphjek.com

TS:   arr.includes(x)
来源：http://zxe.meibo888.top

Java: list.contains(x)
来源：http://zoi.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://tkl.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://eys.zhengqikj.top

C#:   list.Contains(x)
来源：http://iip.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://fzg.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ltn.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jtb.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rqt.0kj1m.cn

TS:   [...arr];
来源：http://kir.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://zfn.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qot.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://dlp.dianchejie.cn

C#:   new List<int>(list);
来源：http://dqu.yuanzhike.top

[D23] reduce 累积计算
来源：http://eci.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mmg.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lkq.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qvb.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znh.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ouc.haohaochexian.top

Go:   // 手写循环
来源：http://bkb.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://irx.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dav.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://stz.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://njk.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://urc.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://chw.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tzl.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tok.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jut.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mei.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lhm.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://jbn.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ctz.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jpf.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fla.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tkp.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hll.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ive.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wov.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://djj.wangdashe.top

[D26] 数组转字符串
来源：http://zea.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://izn.meibo888.top

PHP:  implode(", ", $arr);
来源：http://plu.smart0.xyz

JS:   arr.join(", ")
来源：http://yld.gotoacloud.top

TS:   arr.join(", ")
来源：http://esf.wangdashe.top

Java: String.join(", ", list)
来源：http://tup.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://ruo.shzxlz.cn

Ruby: arr.join(", ")
来源：http://uys.yonumen.top

C#:   string.Join(", ", list)
来源：http://ifb.dianchejie.cn

================================================================================
来源：http://yku.sxryk.cn

E. 字符串处理
来源：http://tew.snrcjt.cn

================================================================================
来源：http://dna.guannengcc.top

[E01] 拼接字符串
来源：http://zgk.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hua.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mwj.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahy.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sno.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pbd.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qqb.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xep.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kqp.zdbjq.cn

[E02] 重复字符串
来源：http://qbj.jianghu66.top

Py:   "ab" * 3
来源：http://vsp.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://okq.sweek.top

JS:   "ab".repeat(3)
来源：http://rnp.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://mtt.yvedp.cn

Java: "ab".repeat(3)
来源：http://iaq.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://mnp.zhongyouzk.top

Ruby: "ab" * 3
来源：http://bwb.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iew.yj202588.top

[E03] 截取子串
来源：http://zaq.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tlx.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://omg.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fuv.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://sga.yuanzhike.top

Java: s.substring(1, 4)
来源：http://lsh.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tzu.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://arm.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://dqb.yvedp.cn

[E04] 查找子串位置
来源：http://bih.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://trw.bbcook.cn

PHP:  strpos($s, "x");
来源：http://wqo.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fzr.tarul.cn

TS:   s.indexOf("x")
来源：http://qlj.uphjek.com

Java: s.indexOf("x")
来源：http://mid.havefunace.top


<!-- 参考信息 -->