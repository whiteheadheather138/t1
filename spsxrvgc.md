代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mey.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ted.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fof.svipenyu.cn

Ruby: # 无泛型
来源：http://nfo.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ryc.daria6918.cn

[C15] 解构 / 展开参数
来源：http://jqv.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://axk.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://vls.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hxi.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nrd.hammf.cn

Java: // 无解构
来源：http://xnr.haohaochexian.top

Go:   // 无解构
来源：http://eux.wangdashe.top

Ruby: a, b = pair
来源：http://bgp.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://lwl.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://zrx.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://has.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://yzt.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://afi.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://vbi.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ndx.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://zun.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://jkq.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://krs.zhiwuduotai.top

================================================================================
来源：http://blt.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://zyq.redwolf501.top

================================================================================
来源：http://xxu.yj20258.top

[D01] 创建数组 / 列表
来源：http://dyd.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://kpj.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mxn.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zde.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fkj.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tlx.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://xmd.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://gqm.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fum.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://zyx.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xpm.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://smg.shangyingyoupin.top

JS:   arr.push(4);
来源：http://xqd.sxryk.cn

TS:   arr.push(4);
来源：http://zld.gogol.net.cn

Java: list.add(4);
来源：http://dff.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://vtz.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://gbm.gzhubu.top

C#:   list.Add(4);
来源：http://iwl.52xcode.cn

[D03] 在指定位置插入元素
来源：http://hxl.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://foc.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bxa.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gne.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://vfz.xziqi.cn

Java: list.add(0, 0);
来源：http://qtp.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vse.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xux.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://kow.wangdashe.top

[D04] 删除元素
来源：http://bva.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vmx.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dwx.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zcn.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://gjs.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xkb.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uof.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://udi.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cka.gotoacloud.top

[D05] 访问与修改元素
来源：http://slh.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sli.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xaf.nanxinkj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sol.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://pce.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://ifj.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://xsr.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ywe.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mcv.yueranfly.top

[D06] 数组长度
来源：http://vwj.guannengcc.top

Py:   len(arr)
来源：http://trc.yj20258888.top

PHP:  count($arr);
来源：http://ukp.cqqwz.cn

JS:   arr.length
来源：http://psf.cdnleiting.top

TS:   arr.length
来源：http://nnh.tian-w.cn

Java: list.size();
来源：http://rrr.gaohongyu789.top

Go:   len(arr)
来源：http://ikh.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://xco.yfazqb.com

C#:   list.Count;
来源：http://xxl.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://bmq.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tec.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://dkx.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://hvk.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://unj.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://hbv.chenlongwang.top

Go:   arr[1:4]
来源：http://caz.jiagoushi.top

Ruby: arr[1, 3]
来源：http://aqq.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://xsh.gzhubu.top

[D08] 合并两个数组
来源：http://eqs.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://ahc.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://rpl.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jri.jqgufenzy.top

TS:   [...a, ...b];
来源：http://nos.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vpk.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://veo.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://yeu.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://ene.ppjwa.cn

[D09] 排序（升序）
来源：http://uhn.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://xmb.jqgfzy.top

PHP:  sort($arr);
来源：http://ejh.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jpo.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fep.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hww.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kpk.daria6918.cn

Ruby: arr.sort
来源：http://kqf.yj20258888.top

C#:   list.Sort();
来源：http://cjm.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zsi.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bfi.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqo.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncw.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fnk.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://grv.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jam.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wwg.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://von.nanxuanxn.top

[D11] 反转数组
来源：http://eof.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rsr.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://fdq.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tio.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://aoa.yangfankeji.com

Java: Collections.reverse(list);
来源：http://byi.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://vux.dianchejie.cn

Ruby: arr.reverse
来源：http://lvh.ppjwa.cn

C#:   list.Reverse();
来源：http://khj.tanke756.top

[D12] 查找元素下标
来源：http://gwt.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://qqc.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ezr.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oye.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkr.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mdc.meibo888.top

Go:   slices.Index(arr, x)
来源：http://tpz.gzhubu.top

Ruby: arr.index(x)
来源：http://pll.havefunace.top

C#:   list.IndexOf(x);
来源：http://zex.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://prg.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://heh.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pxm.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://wae.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://zka.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://stm.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kaw.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://bcl.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dnk.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://hdg.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hjl.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xsa.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://ycj.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://pgd.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jnu.ydzc1.top

Go:   // 手写循环
来源：http://ybh.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gan.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yzo.sjlbkw.cn

[D15] 去重
来源：http://bgk.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jud.0kj1m.cn

PHP:  array_unique($arr);
来源：http://yvv.cashguo.top

JS:   [...new Set(arr)]
来源：http://zvx.iojbl.cn

TS:   [...new Set(arr)]
来源：http://xwl.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ddu.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://gmw.xuanzx.com

Ruby: arr.uniq
来源：http://xpc.cheryme.top

C#:   list.Distinct().ToList()
来源：http://iic.fehbvm.com

[D16] 求和与平均值
来源：http://ndj.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mez.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cbl.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eck.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrm.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kie.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://ywr.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wss.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://opm.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://pea.uphjek.com

Py:   max(arr);  min(arr)
来源：http://jqb.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://hye.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fcz.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://apv.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xpw.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exw.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://ovo.yonumen.top

C#:   list.Max();  list.Min()
来源：http://ztk.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://boz.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dzm.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://pmw.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jtu.meibo888.top

TS:   nested.flat();
来源：http://mox.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ruf.yuanzhike.top

Go:   // 手写双层循环
来源：http://vib.guowangkeji.top

Ruby: nested.flatten
来源：http://fnm.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cln.jlsjyb.cn

[D19] 按字段分组
来源：http://nmu.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://suz.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pod.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://etb.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://imm.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oxx.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://xad.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://yks.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rcx.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://nnc.yongpay.top

Py:   Counter(arr)
来源：http://kyf.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://hhx.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdd.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvb.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vpz.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://uhq.hfpthk.cn

Ruby: arr.tally
来源：http://mnu.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://juf.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://gom.jqgufenzy.top

Py:   x in arr
来源：http://tqq.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://bwz.jinqigufen.top

JS:   arr.includes(x)
来源：http://ywj.jqgufenzy.top

TS:   arr.includes(x)
来源：http://wzn.jlsjyb.cn

Java: list.contains(x)
来源：http://nqy.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://dwb.nanxinkj.top

Ruby: arr.include?(x)
来源：http://eyg.zhijiandao.cn

C#:   list.Contains(x)
来源：http://akh.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://fgf.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jtq.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rsu.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ils.yuxming.cn

TS:   [...arr];
来源：http://doc.cheryme.top

Java: new ArrayList<>(list);
来源：http://enm.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://yai.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://ccz.yonumen.top

C#:   new List<int>(list);
来源：http://nwc.yueranfly.top

[D23] reduce 累积计算
来源：http://ouq.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://osz.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ldx.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fok.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqi.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vxv.ivvv.top

Go:   // 手写循环
来源：http://ifi.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zps.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qse.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://nbc.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wdj.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://myn.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ici.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hsg.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://afz.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zjv.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://alr.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://csl.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://cqz.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mcs.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uoa.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vqy.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uhc.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tod.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqf.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://etn.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cyb.hammf.cn

[D26] 数组转字符串
来源：http://pjs.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://ggu.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://cnw.cheryme.top

JS:   arr.join(", ")
来源：http://noz.gaohongyu789.top

TS:   arr.join(", ")
来源：http://sgh.mhx1999.top

Java: String.join(", ", list)
来源：http://frx.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://jgd.chenlongwang.top

Ruby: arr.join(", ")
来源：http://qbn.xziqi.cn

C#:   string.Join(", ", list)
来源：http://qwz.zdqjudy.top

================================================================================
来源：http://veu.shzxlz.cn

E. 字符串处理
来源：http://plv.hongshengwenyu.top

================================================================================
来源：http://aiu.yj202588.top

[E01] 拼接字符串
来源：http://zwu.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aro.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://srd.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nbh.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dip.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://opb.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xfs.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://euo.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uat.jinqigfzy.top

[E02] 重复字符串
来源：http://miz.ydjk.org.cn

Py:   "ab" * 3
来源：http://ybp.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://vcv.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://bci.yuxming.cn

TS:   "ab".repeat(3)
来源：http://qtm.yangfankeji.com

Java: "ab".repeat(3)
来源：http://hbh.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://ush.yangfankeji.com

Ruby: "ab" * 3
来源：http://rlv.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rit.pengpengdd.cyou

[E03] 截取子串
来源：http://kwf.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ohu.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cee.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://avh.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://kbh.daria6918.cn

Java: s.substring(1, 4)
来源：http://dbr.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bdq.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qoh.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://swu.shangyingyoupin.top

[E04] 查找子串位置
来源：http://xlz.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://qhg.shuidangran.top

PHP:  strpos($s, "x");
来源：http://gmm.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ths.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://yqv.jinqigfzy.top

Java: s.indexOf("x")
来源：http://prj.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://wrb.shzxlz.cn

Ruby: s.index("x")
来源：http://iqc.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://tpq.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kow.hcnkem.com


<!-- 参考信息 -->