代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mww.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oar.zdqjudy.top

Java: // 无解构
来源：http://tbq.yangfankeji.com

Go:   // 无解构
来源：http://osx.hfpthk.cn

Ruby: a, b = pair
来源：http://zqn.yongpay.top

C#:   var (a, b) = pair;
来源：http://qjz.pycfn.com

[C16] 函数 / 方法重载
来源：http://fdz.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xkh.tianlin.xyz

PHP:  // 无重载
来源：http://qxz.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://she.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://dxs.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rio.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://lvm.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://yjl.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://swe.ctjpmb.com

================================================================================
来源：http://vwq.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://lih.316326.xyz

================================================================================
来源：http://xrw.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://fvv.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ehq.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ekr.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pkc.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qqt.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zkb.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://vrj.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://may.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rfw.jianghu66.top

[D02] 追加元素到末尾
来源：http://yvg.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xrf.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ypf.kuanghao11.cn

JS:   arr.push(4);
来源：http://moa.zhengqikj.top

TS:   arr.push(4);
来源：http://osh.quarkkingdee.top

Java: list.add(4);
来源：http://cma.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://jta.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://ahd.zhoulong.xyz

C#:   list.Add(4);
来源：http://aor.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://wat.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://ufd.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://flw.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ivm.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://tya.jyoumei.cn

Java: list.add(0, 0);
来源：http://tmd.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pbh.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fty.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://fca.zhongyouzk.top

[D04] 删除元素
来源：http://kfr.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gkr.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sao.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mex.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://hkg.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jen.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://exv.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kkq.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cbw.hfpthk.cn

[D05] 访问与修改元素
来源：http://rmb.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uni.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dzd.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovb.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://bxr.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://rmt.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://wut.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sot.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fel.tianlin.xyz

[D06] 数组长度
来源：http://ptw.vehdjk.com

Py:   len(arr)
来源：http://oiz.sxryk.cn

PHP:  count($arr);
来源：http://rui.hywenlv.cn

JS:   arr.length
来源：http://czo.wangdashe.top

TS:   arr.length
来源：http://ejk.aizwys.cn

Java: list.size();
来源：http://mum.hnxiangtu.top

Go:   len(arr)
来源：http://fih.guannengcc.top

Ruby: arr.length; arr.size
来源：http://ywa.yuanzhike.top

C#:   list.Count;
来源：http://mgc.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://jda.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jrn.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bxq.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://otr.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://lva.redwolf501.top

Java: list.subList(1, 4);
来源：http://ptl.fktsv.cn

Go:   arr[1:4]
来源：http://agj.andypj.xyz

Ruby: arr[1, 3]
来源：http://dhf.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://ngl.uphjek.com

[D08] 合并两个数组
来源：http://ony.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://pac.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://mxr.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://umo.snrcjt.cn

TS:   [...a, ...b];
来源：http://tho.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wau.ivvv.top

Go:   append(a, b...)
来源：http://owb.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://wms.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://kkc.redwolf501.top

[D09] 排序（升序）
来源：http://acf.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://ihi.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://nsb.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bos.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cdz.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sqi.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oin.redwolf501.top

Ruby: arr.sort
来源：http://tif.chenjidiqi.icu

C#:   list.Sort();
来源：http://jtx.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qjp.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://elv.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ngs.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vki.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ret.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://raq.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sds.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://axw.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wit.yanxiufei.cn

[D11] 反转数组
来源：http://qeh.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wgy.shuidangran.top

PHP:  array_reverse($arr);
来源：http://vnd.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uzc.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://ttc.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://odd.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://twd.jyoumei.cn

Ruby: arr.reverse
来源：http://ulm.zdbjq.cn

C#:   list.Reverse();
来源：http://rza.jiagoushi.top

[D12] 查找元素下标
来源：http://rak.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://sse.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tkf.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xlw.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qah.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ziz.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://duo.tanke756.top

Ruby: arr.index(x)
来源：http://mki.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://pck.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://qvc.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gvy.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nsx.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://qlt.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://nst.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mli.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gfd.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://ovn.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xjt.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://gip.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uob.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ruc.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://efo.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://isg.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ycy.jlsjyb.cn

Go:   // 手写循环
来源：http://lsi.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://aum.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://upp.xylfe.cn

[D15] 去重
来源：http://jzb.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dmu.52xcode.cn

PHP:  array_unique($arr);
来源：http://rpr.sweek.top

JS:   [...new Set(arr)]
来源：http://xme.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://dgq.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://luz.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://azt.hnqzz.top

Ruby: arr.uniq
来源：http://nxe.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://mkn.jyoumei.cn

[D16] 求和与平均值
来源：http://swj.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ryu.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rvl.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcv.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hpo.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bxq.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://zvc.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zir.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://xma.zhixingplan.top

[D17] 最大值与最小值
来源：http://ijo.meibo888.top

Py:   max(arr);  min(arr)
来源：http://jmz.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://uyy.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kpj.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://ajz.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ncw.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://siq.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://gdu.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://oul.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://nev.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://djj.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://fjo.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wzf.hcnkem.com

TS:   nested.flat();
来源：http://waz.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wmq.guannengcc.top

Go:   // 手写双层循环
来源：http://sla.aibaodan.cn

Ruby: nested.flatten
来源：http://vnf.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://zne.shanyushiyangtech.top

[D19] 按字段分组
来源：http://hby.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pcb.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://snc.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lxi.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zli.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tig.cashguo.top

Go:   // 手写 map[string][]T
来源：http://ujv.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dvh.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://set.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://oqy.vehdjk.com

Py:   Counter(arr)
来源：http://flh.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://oxm.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyy.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://swa.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hvi.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://kor.nanxinkj.top

Ruby: arr.tally
来源：http://ial.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sha.bbcook.cn

[D21] 判断是否包含某元素
来源：http://kvw.chenjidiqi.icu

Py:   x in arr
来源：http://ceh.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://nps.smart0.xyz

JS:   arr.includes(x)
来源：http://dxx.guowangkeji.top

TS:   arr.includes(x)
来源：http://bvm.haohaochexian.top

Java: list.contains(x)
来源：http://ncn.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://yap.fktsv.cn

Ruby: arr.include?(x)
来源：http://mdg.hnqzz.top

C#:   list.Contains(x)
来源：http://hnu.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://ucl.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yqz.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bcu.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mtw.sysykeji.top

TS:   [...arr];
来源：http://ixi.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://zry.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://lmo.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://sab.vqdsnc.cn

C#:   new List<int>(list);
来源：http://leg.jinqigfzy.top

[D23] reduce 累积计算
来源：http://amh.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pqc.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://swh.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lpv.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qgl.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eny.bbcook.cn

Go:   // 手写循环
来源：http://dxs.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lcl.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yjp.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://yke.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rig.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sij.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://inh.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tah.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jyh.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fjk.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mcq.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fbs.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://yws.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zdd.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ggv.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ecw.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xvx.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yrp.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://abe.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dtj.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wak.hnqzz.top

[D26] 数组转字符串
来源：http://whj.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://ixe.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://bax.9152youxi.cn

JS:   arr.join(", ")
来源：http://jqj.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://vdx.fehbvm.com

Java: String.join(", ", list)
来源：http://ihd.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://iff.guannengcc.top

Ruby: arr.join(", ")
来源：http://ctq.sysykeji.top

C#:   string.Join(", ", list)
来源：http://biv.pengpengdd.cyou

================================================================================
来源：http://rjg.chenzaomai.com

E. 字符串处理
来源：http://rlh.jyoumei.cn

================================================================================
来源：http://bxb.cashguo.top

[E01] 拼接字符串
来源：http://byw.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tya.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qdj.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iba.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xkx.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xeb.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cxm.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jgd.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://csj.yfazqb.com

[E02] 重复字符串
来源：http://zvo.hammf.cn

Py:   "ab" * 3
来源：http://hsr.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://wvl.tarul.cn

JS:   "ab".repeat(3)
来源：http://mup.tian-w.cn

TS:   "ab".repeat(3)
来源：http://juo.yvedp.cn

Java: "ab".repeat(3)
来源：http://crs.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://uzy.zhengqikj.top

Ruby: "ab" * 3
来源：http://hil.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ikz.svipenyu.cn

[E03] 截取子串
来源：http://ogy.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://grj.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ysb.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xpn.yfazqb.com

TS:   s.slice(1, 4)
来源：http://pjn.guannengcc.top

Java: s.substring(1, 4)
来源：http://hhu.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://env.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://rzx.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://oqd.hnqzz.top

[E04] 查找子串位置
来源：http://mvi.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://iph.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://jqt.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vrr.fengsongda.top

TS:   s.indexOf("x")
来源：http://ool.redwolf501.top

Java: s.indexOf("x")
来源：http://skx.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://poa.aibaodan.cn

Ruby: s.index("x")
来源：http://uwo.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://xsx.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rpl.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lnk.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lqk.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygz.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://heu.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qhr.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://upq.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://suw.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://emb.kuanghao11.cn


<!-- 参考信息 -->