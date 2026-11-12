代发 wailian999

D. 数组 / 列表 / 集合
来源：http://dca.dianchejie.cn

================================================================================
来源：http://sgc.daxiang520.top

[D01] 创建数组 / 列表
来源：http://ato.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://isa.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gsf.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jcg.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vlw.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kof.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://llq.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://hdk.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nju.yj20258.top

[D02] 追加元素到末尾
来源：http://tjz.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://okq.jianghu66.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cas.zhengqikj.top

JS:   arr.push(4);
来源：http://wjy.zhiwuduotai.top

TS:   arr.push(4);
来源：http://kei.uphjek.com

Java: list.add(4);
来源：http://zao.hammf.cn

Go:   arr = append(arr, 4)
来源：http://asm.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://inx.0kj1m.cn

C#:   list.Add(4);
来源：http://skn.smart0.xyz

[D03] 在指定位置插入元素
来源：http://lta.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://icg.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fvl.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lkq.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://yhe.redwolf501.top

Java: list.add(0, 0);
来源：http://clb.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://uax.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kjz.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://etr.hnxiangtu.top

[D04] 删除元素
来源：http://tov.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ced.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tpj.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ktr.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://slo.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lmz.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://edw.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pnj.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zli.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://can.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jfq.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hlw.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nni.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://vwm.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://gip.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://xfg.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jew.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxr.redwolf501.top

[D06] 数组长度
来源：http://rew.shanyushiyangkeji.top

Py:   len(arr)
来源：http://wnk.tian-w.cn

PHP:  count($arr);
来源：http://bnb.yuanzhike.top

JS:   arr.length
来源：http://hsc.zhongyouzk.top

TS:   arr.length
来源：http://qdt.gogol.net.cn

Java: list.size();
来源：http://nxg.fktsv.cn

Go:   len(arr)
来源：http://jca.yuxming.cn

Ruby: arr.length; arr.size
来源：http://nis.jinghuilouyu.cn

C#:   list.Count;
来源：http://egq.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://bts.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jlb.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://ifj.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://gfp.cashguo.top

TS:   arr.slice(1, 4);
来源：http://bvl.jyoumei.cn

Java: list.subList(1, 4);
来源：http://pqf.aizwys.cn

Go:   arr[1:4]
来源：http://xlb.cashguo.top

Ruby: arr[1, 3]
来源：http://kag.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://ehs.cucudq.cn

[D08] 合并两个数组
来源：http://wol.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://wvm.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://gfs.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bub.gzhubu.top

TS:   [...a, ...b];
来源：http://vlu.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lbb.zdbjq.cn

Go:   append(a, b...)
来源：http://ycz.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://ljv.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://rbz.hammf.cn

[D09] 排序（升序）
来源：http://maz.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ttk.wangdashe.top

PHP:  sort($arr);
来源：http://rht.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uxz.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dic.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mqq.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pun.ydzc1.top

Ruby: arr.sort
来源：http://pix.gogol.net.cn

C#:   list.Sort();
来源：http://ynw.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mwk.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://csr.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cse.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntg.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nim.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wqh.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dhw.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sfk.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://svl.yj20258.top

[D11] 反转数组
来源：http://xzh.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://uho.yj20258.top

PHP:  array_reverse($arr);
来源：http://hut.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://igc.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://fgd.jqgfzy.top

Java: Collections.reverse(list);
来源：http://txn.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://tyd.fzhhl.top

Ruby: arr.reverse
来源：http://fwj.xuanzx.com

C#:   list.Reverse();
来源：http://toa.wangshuangyany.cn

[D12] 查找元素下标
来源：http://jtu.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://loc.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wvv.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://amx.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wnr.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gih.cheryme.top

Go:   slices.Index(arr, x)
来源：http://voh.hesvh.cn

Ruby: arr.index(x)
来源：http://tia.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://vbo.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://ugu.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://isr.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zcl.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://hgx.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://mbe.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fhl.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bhx.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://wni.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://hmd.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://yqg.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vxb.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://stt.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://oco.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://ipb.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yoq.tanke756.top

Go:   // 手写循环
来源：http://aiz.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vbo.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://umb.tianlin.xyz

[D15] 去重
来源：http://lzl.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sfo.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://lod.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://khp.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://qjh.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vwv.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://hua.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://umf.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://glt.svipenyu.cn

[D16] 求和与平均值
来源：http://mxv.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gds.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yew.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fvq.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hou.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vze.nanxinkj.top

Go:   // 手写循环累加
来源：http://jmp.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qhv.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://gst.meibo888.top

[D17] 最大值与最小值
来源：http://bks.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://txs.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://wpi.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://noo.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://cdh.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://opo.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bgi.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://pbm.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://wng.pycfn.com

[D18] 扁平化嵌套数组
来源：http://ugn.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yzl.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://tki.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://idu.dashuyun.cn

TS:   nested.flat();
来源：http://ydo.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://who.zhijiandao.cn

Go:   // 手写双层循环
来源：http://tnl.quarkkingdee.top

Ruby: nested.flatten
来源：http://anx.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sgx.zhongyouzk.top

[D19] 按字段分组
来源：http://tkw.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tfx.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wpl.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ogg.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://jmv.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bln.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://fzo.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ozw.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ywr.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://zna.epnwcf.com

Py:   Counter(arr)
来源：http://lvm.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://dlk.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dss.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvd.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dwj.daria6918.cn

Go:   // 手写 map[T]int
来源：http://uif.feifeiyinyue.top

Ruby: arr.tally
来源：http://oem.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kqd.xuanzx.com

[D21] 判断是否包含某元素
来源：http://bzb.shangyingyoupin.top

Py:   x in arr
来源：http://prk.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://jqm.fengsongda.top

JS:   arr.includes(x)
来源：http://glc.jqgufenzy.top

TS:   arr.includes(x)
来源：http://whe.wangdashe.top

Java: list.contains(x)
来源：http://rqo.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://xcc.hysaishi.cn

Ruby: arr.include?(x)
来源：http://nih.jiagoushi.top

C#:   list.Contains(x)
来源：http://pxf.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://ugy.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mgw.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ouv.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mnv.xziqi.cn

TS:   [...arr];
来源：http://cpc.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://btc.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zfp.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://faf.gotoacloud.top

C#:   new List<int>(list);
来源：http://brl.ydjk.org.cn

[D23] reduce 累积计算
来源：http://zeh.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xwf.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xnd.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lab.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gau.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bqo.xziqi.cn

Go:   // 手写循环
来源：http://sii.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zrl.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ixd.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://geq.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yjn.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vyc.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ocf.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mui.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oxe.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eoo.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lug.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kag.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://kff.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ftz.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oij.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://exp.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kbb.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oip.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bzc.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bwm.pycfn.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tiy.xinyue.icu

[D26] 数组转字符串
来源：http://rlt.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://ncv.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://crz.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://dfg.haohaochexian.top

TS:   arr.join(", ")
来源：http://yws.316326.xyz

Java: String.join(", ", list)
来源：http://mof.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://tcu.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://swu.yvedp.cn

C#:   string.Join(", ", list)
来源：http://nin.dashuyun.cn

================================================================================
来源：http://tyj.yuxming.cn

E. 字符串处理
来源：http://tim.epnwcf.com

================================================================================
来源：http://knw.ivvv.top

[E01] 拼接字符串
来源：http://dkb.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zfz.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nsu.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dfn.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hry.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dbv.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ztd.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ufm.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wwt.dashuyun.cn

[E02] 重复字符串
来源：http://fda.yangfankeji.com

Py:   "ab" * 3
来源：http://aut.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://qnu.daxiang520.top

JS:   "ab".repeat(3)
来源：http://yeb.fehbvm.com

TS:   "ab".repeat(3)
来源：http://laq.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://oem.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://wvo.birdmap.top

Ruby: "ab" * 3
来源：http://evw.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xff.wangshuangyany.cn

[E03] 截取子串
来源：http://qjx.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rhq.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wbm.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://teu.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://jku.snrcjt.cn

Java: s.substring(1, 4)
来源：http://hzx.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hqa.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://hno.pycfn.com

C#:   s.Substring(1, 3)
来源：http://fdw.hfpthk.cn

[E04] 查找子串位置
来源：http://gqo.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://gjb.yueranfly.top

PHP:  strpos($s, "x");
来源：http://ssi.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hbi.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://ebe.xylfe.cn

Java: s.indexOf("x")
来源：http://kcd.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://fgw.zdbjq.cn

Ruby: s.index("x")
来源：http://ybw.hysaishi.cn

C#:   s.IndexOf("x")
来源：http://nod.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nzu.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fuy.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rft.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dkn.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kcb.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hon.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xvs.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vov.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lhe.jianghu66.top

[E06] 替换子串
来源：http://gyz.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kvf.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://dza.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cdq.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://qcx.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lmx.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://goy.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bqh.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://rbi.yangfankeji.com

[E07] 按分隔符拆分
来源：http://lwn.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vdm.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eqc.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://wqh.snrcjt.cn

TS:   s.split(",")
来源：http://vxr.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://iiv.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jkc.9152youxi.cn


<!-- 参考信息 -->