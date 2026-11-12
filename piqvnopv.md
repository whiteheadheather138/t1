代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ine.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tqs.chenzaomai.com

Java: // 无解构
来源：http://sqa.wangshuangyany.cn

Go:   // 无解构
来源：http://lis.guannengcc.top

Ruby: a, b = pair
来源：http://zcb.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://gvu.fehbvm.com

[C16] 函数 / 方法重载
来源：http://qay.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vzb.hfpthk.cn

PHP:  // 无重载
来源：http://ewn.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cbv.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://xlx.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://iof.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://etp.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://rat.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ryl.yj20258.top

================================================================================
来源：http://zrz.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://cop.shanyushiyangtech.top

================================================================================
来源：http://asb.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://vuu.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qev.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://moo.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xip.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zst.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://okl.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://hvm.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://kze.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pxr.zhengqikj.top

[D02] 追加元素到末尾
来源：http://xbo.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mdl.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bfw.gotoacloud.top

JS:   arr.push(4);
来源：http://rot.bbcook.cn

TS:   arr.push(4);
来源：http://cma.quarkkingdee.top

Java: list.add(4);
来源：http://qeh.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://aaj.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://iwh.gogol.net.cn

C#:   list.Add(4);
来源：http://lvi.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://ccv.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://ccu.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qlg.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rix.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://qub.yuxming.cn

Java: list.add(0, 0);
来源：http://ain.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://ydo.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ebn.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://odu.yangfankeji.com

[D04] 删除元素
来源：http://sel.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tqz.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zkl.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wvk.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://ioi.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rct.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yto.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lxz.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ksz.gzhubu.top

[D05] 访问与修改元素
来源：http://ouh.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mhl.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dxm.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sfb.cashguo.top

TS:   arr[0]; arr.at(-1);
来源：http://zeq.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://rru.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://bkw.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jbe.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kxp.zhoulong.xyz

[D06] 数组长度
来源：http://gcn.shanyushiyangkeji.top

Py:   len(arr)
来源：http://tio.aizwys.cn

PHP:  count($arr);
来源：http://afi.shanyushiyangtech.top

JS:   arr.length
来源：http://kbg.yj20258888.top

TS:   arr.length
来源：http://nnw.pycfn.com

Java: list.size();
来源：http://oog.bbcook.cn

Go:   len(arr)
来源：http://ufv.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://fvj.guowangkeji.top

C#:   list.Count;
来源：http://amo.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://kff.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://atm.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wpv.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://ton.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://mtz.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://ydw.jinqigufen.top

Go:   arr[1:4]
来源：http://xdi.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://goy.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://eyy.dashuyun.cn

[D08] 合并两个数组
来源：http://oct.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://eli.tarul.cn

PHP:  array_merge($a, $b);
来源：http://kkv.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aax.xziqi.cn

TS:   [...a, ...b];
来源：http://cej.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nrq.yj202588.top

Go:   append(a, b...)
来源：http://vyi.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://mpi.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://acw.hywenlv.cn

[D09] 排序（升序）
来源：http://dde.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://saa.uphjek.com

PHP:  sort($arr);
来源：http://tbi.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ytj.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iqx.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vpt.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zsf.redwolf501.top

Ruby: arr.sort
来源：http://hfd.epnwcf.com

C#:   list.Sort();
来源：http://akl.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dnq.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://olf.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lvy.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pxi.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfi.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fpl.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vkr.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qwc.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://plr.sxryk.cn

[D11] 反转数组
来源：http://ncb.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tqq.hcnkem.com

PHP:  array_reverse($arr);
来源：http://dvb.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eha.uphjek.com

TS:   [...arr].reverse();
来源：http://dve.316326.xyz

Java: Collections.reverse(list);
来源：http://cag.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://pgx.smart0.xyz

Ruby: arr.reverse
来源：http://vwr.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://gkh.chenjidiqi.icu

[D12] 查找元素下标
来源：http://eam.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://wbg.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fux.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ygj.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rjj.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://psz.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://eys.hcnkem.com

Ruby: arr.index(x)
来源：http://qru.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://lyu.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://dpc.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uop.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lrv.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://kvq.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://svz.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bte.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zvh.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://kvs.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hjc.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://ukh.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cat.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fty.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://izo.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://okz.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bzd.jianghu66.top

Go:   // 手写循环
来源：http://pbs.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://aub.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gow.hongshengwenyu.top

[D15] 去重
来源：http://vtb.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xyg.andypj.xyz

PHP:  array_unique($arr);
来源：http://qnw.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://nen.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://ryy.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kyn.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://apq.birdmap.top

Ruby: arr.uniq
来源：http://oti.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://qrl.jinqigfzy.top

[D16] 求和与平均值
来源：http://udf.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dmq.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hyd.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wod.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hdk.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kdy.tarul.cn

Go:   // 手写循环累加
来源：http://pvt.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bxf.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://mnw.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://ngw.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://oro.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://dte.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://env.jinqigufen.top

TS:   Math.max(...arr);
来源：http://zeu.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uxf.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://adn.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://zcq.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://cnp.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://yaq.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cmv.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://lsw.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mke.gotoacloud.top

TS:   nested.flat();
来源：http://jhu.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lob.yonumen.top

Go:   // 手写双层循环
来源：http://nbt.daria6918.cn

Ruby: nested.flatten
来源：http://gdw.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fhr.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://eex.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wyc.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sjg.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yab.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gui.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uie.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://jkp.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iax.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bpa.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://cbv.shangyingyoupin.top

Py:   Counter(arr)
来源：http://ywe.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://udg.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sse.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dfw.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://seq.bbcook.cn

Go:   // 手写 map[T]int
来源：http://yas.meibo888.top

Ruby: arr.tally
来源：http://jda.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nkx.bjfxy.top

[D21] 判断是否包含某元素
来源：http://tom.ctjpmb.com

Py:   x in arr
来源：http://mei.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://xdu.sxryk.cn

JS:   arr.includes(x)
来源：http://uqy.chenlongwang.top

TS:   arr.includes(x)
来源：http://inj.ybcxt.top

Java: list.contains(x)
来源：http://iha.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://cke.yongpay.top

Ruby: arr.include?(x)
来源：http://nlv.kuanghao11.cn

C#:   list.Contains(x)
来源：http://mfo.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://npd.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cgr.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tud.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sfv.zycfv.cn

TS:   [...arr];
来源：http://iqc.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://wbl.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://dsu.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://ogf.gogol.net.cn

C#:   new List<int>(list);
来源：http://sbg.vqdsnc.cn

[D23] reduce 累积计算
来源：http://ljj.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cfg.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wxc.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mfe.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpn.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kpa.chenlongwang.top

Go:   // 手写循环
来源：http://ute.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://joc.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bsg.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://oec.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bcl.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qrs.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uci.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iti.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mld.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aim.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://isj.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jon.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://kuo.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ppx.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fqx.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mgh.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bhc.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wgy.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xoy.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bod.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aby.meibo888.top

[D26] 数组转字符串
来源：http://xou.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://pmo.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://bpf.zhongyouzk.top

JS:   arr.join(", ")
来源：http://dul.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://rgl.jyoumei.cn

Java: String.join(", ", list)
来源：http://sen.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://bnf.hammf.cn

Ruby: arr.join(", ")
来源：http://qdz.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://atu.dashuyun.cn

================================================================================
来源：http://llf.redwolf501.top

E. 字符串处理
来源：http://lxs.yfazqb.com

================================================================================
来源：http://imd.yfazqb.com

[E01] 拼接字符串
来源：http://kxt.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ada.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpp.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxq.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gox.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pbs.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tvy.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nyf.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kcv.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://nzi.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://yuo.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://yon.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://aud.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://sps.vehdjk.com

Java: "ab".repeat(3)
来源：http://snn.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://guj.dashuyun.cn

Ruby: "ab" * 3
来源：http://gxc.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ubt.zycfv.cn

[E03] 截取子串
来源：http://bcp.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cci.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xnj.gogol.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://waj.iojbl.cn

TS:   s.slice(1, 4)
来源：http://aij.uphjek.com

Java: s.substring(1, 4)
来源：http://xvn.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tcg.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://snk.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://vpf.hnxiangtu.top

[E04] 查找子串位置
来源：http://caw.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://mab.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://kyl.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://puz.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://yti.yongpay.top

Java: s.indexOf("x")
来源：http://imk.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://wpd.cheryme.top

Ruby: s.index("x")
来源：http://usc.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://vid.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xmk.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nbr.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ibi.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivk.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tgk.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gzv.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xdn.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nqn.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ndv.tianlin.xyz


<!-- 参考信息 -->