代发 wailian999

PHP:  // 无重载
来源：http://smi.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pzw.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://wgg.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ltj.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://dmk.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://afb.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mcm.jinqigufen.top

================================================================================
来源：http://jzw.ivvv.top

D. 数组 / 列表 / 集合
来源：http://xdo.ehwqpu.com

================================================================================
来源：http://dyt.jianghu66.top

[D01] 创建数组 / 列表
来源：http://bwh.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vid.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://upz.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mbw.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tfd.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qbj.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://wus.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://pao.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ddd.vehdjk.com

[D02] 追加元素到末尾
来源：http://zup.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wpz.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iwa.fengsongda.top

JS:   arr.push(4);
来源：http://vsv.yfazqb.com

TS:   arr.push(4);
来源：http://jiq.tianlin.xyz

Java: list.add(4);
来源：http://xqw.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://wrm.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://ikq.andypj.xyz

C#:   list.Add(4);
来源：http://hut.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://kcc.ivvv.top

Py:   arr.insert(0, 0)
来源：http://qcs.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zno.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cmq.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://sbh.zhixingplan.top

Java: list.add(0, 0);
来源：http://umk.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jmq.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xci.yongpay.top

C#:   list.Insert(0, 0);
来源：http://dqo.fktsv.cn

[D04] 删除元素
来源：http://gbx.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wtt.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ggl.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://huz.yonumen.top

TS:   arr.splice(0, 1);
来源：http://gjz.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bno.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rnf.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ifb.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://via.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://jzz.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qys.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dwf.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zfn.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://kku.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://pvr.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://roq.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://glk.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pou.haohaochexian.top

[D06] 数组长度
来源：http://afx.iojbl.cn

Py:   len(arr)
来源：http://yfk.cucudq.cn

PHP:  count($arr);
来源：http://fco.yj202588.top

JS:   arr.length
来源：http://wej.yuxming.cn

TS:   arr.length
来源：http://ddb.sufxvd.cn

Java: list.size();
来源：http://flz.fehbvm.com

Go:   len(arr)
来源：http://zgf.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://vow.svipenyu.cn

C#:   list.Count;
来源：http://lkc.aizwys.cn

[D07] 切片 / 取子数组
来源：http://ewd.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fzv.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://qix.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://mdg.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://jks.jiagoushi.top

Java: list.subList(1, 4);
来源：http://buc.jqgufenzy.top

Go:   arr[1:4]
来源：http://acu.xylfe.cn

Ruby: arr[1, 3]
来源：http://oqn.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://usj.zhixingplan.top

[D08] 合并两个数组
来源：http://bke.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://fry.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://gmi.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ser.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://uae.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rib.pengpengdd.cyou

Go:   append(a, b...)
来源：http://dle.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://wrr.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://bzt.sjlbkw.cn

[D09] 排序（升序）
来源：http://wfm.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://qhc.ehwqpu.com

PHP:  sort($arr);
来源：http://oky.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rqp.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://dsq.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ubv.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rru.gotoacloud.top

Ruby: arr.sort
来源：http://lyf.sxryk.cn

C#:   list.Sort();
来源：http://zca.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ibi.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wze.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqi.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oot.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pul.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fiz.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qio.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nkz.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dlk.xinyue.icu

[D11] 反转数组
来源：http://pyh.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fpe.guannengcc.top

PHP:  array_reverse($arr);
来源：http://ycl.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://coo.0kj1m.cn

TS:   [...arr].reverse();
来源：http://mio.hfpthk.cn

Java: Collections.reverse(list);
来源：http://zyu.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://ukp.yueranfly.top

Ruby: arr.reverse
来源：http://ekd.sxryk.cn

C#:   list.Reverse();
来源：http://obf.iojbl.cn

[D12] 查找元素下标
来源：http://vto.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://nij.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nfe.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pdj.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxm.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mqw.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://nap.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://zbz.smart0.xyz

C#:   list.IndexOf(x);
来源：http://rqa.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://vot.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://von.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ctz.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://tyx.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://fye.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qla.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ypv.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://wmc.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tix.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://vvb.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xpu.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://paw.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://xbm.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://vrn.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lmw.svipenyu.cn

Go:   // 手写循环
来源：http://foq.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fap.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qgd.hfpthk.cn

[D15] 去重
来源：http://ovl.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kic.iojbl.cn

PHP:  array_unique($arr);
来源：http://vyt.fzhhl.top

JS:   [...new Set(arr)]
来源：http://vko.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://wzs.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uws.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://sqb.havefunace.top

Ruby: arr.uniq
来源：http://wry.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://ffb.sxryk.cn

[D16] 求和与平均值
来源：http://cit.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://odi.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qtd.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuu.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://msx.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://trz.yj20258.top

Go:   // 手写循环累加
来源：http://uto.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qpe.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://rra.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://ozg.yongpay.top

Py:   max(arr);  min(arr)
来源：http://ygy.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://wsp.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fgy.tanke756.top

TS:   Math.max(...arr);
来源：http://uft.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nia.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oak.sweek.top

Ruby: arr.max;  arr.min
来源：http://emn.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://meq.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://thd.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sqe.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://zkq.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ick.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://hly.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sgn.andypj.xyz

Go:   // 手写双层循环
来源：http://zls.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://jpk.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tdm.hnxiangtu.top

[D19] 按字段分组
来源：http://evk.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tuq.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rqg.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sze.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pqz.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pvm.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://iqh.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyn.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fsb.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://hko.hysaishi.cn

Py:   Counter(arr)
来源：http://htc.fzhhl.top

PHP:  array_count_values($arr);
来源：http://owk.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ahu.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erp.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fsd.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://sfo.hnxiangtu.top

Ruby: arr.tally
来源：http://pqp.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ccv.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://dnp.ywan-chungtsiang.top

Py:   x in arr
来源：http://khs.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://obr.ehwqpu.com

JS:   arr.includes(x)
来源：http://hbs.hnqzz.top

TS:   arr.includes(x)
来源：http://jha.yj20258.top

Java: list.contains(x)
来源：http://fjw.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://hkr.ctjpmb.com

Ruby: arr.include?(x)
来源：http://enc.chenlongwang.top

C#:   list.Contains(x)
来源：http://tfi.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://rri.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fdj.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ykj.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cgr.sufxvd.cn

TS:   [...arr];
来源：http://tqg.jlsjyb.cn

Java: new ArrayList<>(list);
来源：http://mux.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://hvw.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://spq.shzxlz.cn

C#:   new List<int>(list);
来源：http://wkb.fzhhl.top

[D23] reduce 累积计算
来源：http://hgd.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://phi.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wli.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qlp.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xnq.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://swb.zdqjudy.top

Go:   // 手写循环
来源：http://qxr.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kgm.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oqi.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://rgs.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fht.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iyt.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pjc.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fwf.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dmq.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fax.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tyc.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://odi.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://nhf.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xwv.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zkj.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mjn.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yvn.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ssw.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lyf.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hyk.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rsr.zhiwuduotai.top

[D26] 数组转字符串
来源：http://vtj.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://axt.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://dkq.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://nqt.jinqigfzy.top

TS:   arr.join(", ")
来源：http://zbj.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://oar.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://ntw.yj20258888.top

Ruby: arr.join(", ")
来源：http://gvm.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://aoq.jinqigfzy.top

================================================================================
来源：http://qmy.bbcook.cn

E. 字符串处理
来源：http://lem.tian-w.cn

================================================================================
来源：http://pvw.haohaochexian.top

[E01] 拼接字符串
来源：http://one.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mxm.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vkb.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ilp.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fdl.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tqy.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kkm.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xnw.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bll.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://kls.vehdjk.com

Py:   "ab" * 3
来源：http://jdu.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://uyr.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://ivp.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://ruw.yfazqb.com

Java: "ab".repeat(3)
来源：http://atq.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://jol.yangfankeji.com

Ruby: "ab" * 3
来源：http://lnk.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nff.zhengqikj.top

[E03] 截取子串
来源：http://qtb.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nwx.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bkc.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bel.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://ovv.sysykeji.top

Java: s.substring(1, 4)
来源：http://xpz.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rjm.9152youxi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ehh.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://zio.yuanzhike.top

[E04] 查找子串位置
来源：http://hzg.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://tan.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://klb.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kja.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://xuf.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://xrr.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://xoq.ydzc1.top

Ruby: s.index("x")
来源：http://uvw.yuxming.cn

C#:   s.IndexOf("x")
来源：http://rcu.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dmj.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://acb.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zlw.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftx.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wcf.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgz.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://imu.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kby.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vgo.dianchejie.cn

[E06] 替换子串
来源：http://war.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bng.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://ozn.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gwh.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://xeg.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhk.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://spq.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dua.yonumen.top


<!-- 参考信息 -->