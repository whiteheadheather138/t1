代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ysh.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://twz.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vqx.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qpx.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://mbp.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://ztu.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zae.jiagoushi.top

[D02] 追加元素到末尾
来源：http://ffq.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vrr.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mgm.epnwcf.com

JS:   arr.push(4);
来源：http://tnj.jiagoushi.top

TS:   arr.push(4);
来源：http://oqx.jiagoushi.top

Java: list.add(4);
来源：http://nzl.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://lea.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://nua.dianchejie.cn

C#:   list.Add(4);
来源：http://qbe.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://nnv.sweek.top

Py:   arr.insert(0, 0)
来源：http://kne.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ayi.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lwx.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://zfx.yueranfly.top

Java: list.add(0, 0);
来源：http://vdh.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ovi.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yky.uphjek.com

C#:   list.Insert(0, 0);
来源：http://pbu.bbcook.cn

[D04] 删除元素
来源：http://bnt.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wmf.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pcj.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pfk.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://hcp.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bxq.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ugr.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jtp.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bka.birdmap.top

[D05] 访问与修改元素
来源：http://kgn.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://taw.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wma.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ues.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://ivi.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://qws.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://yvi.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zjq.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dnk.fehbvm.com

[D06] 数组长度
来源：http://tsd.ydjk.org.cn

Py:   len(arr)
来源：http://tek.sufxvd.cn

PHP:  count($arr);
来源：http://knr.ydzc1.top

JS:   arr.length
来源：http://edw.yj202588.top

TS:   arr.length
来源：http://rwu.tianlin.xyz

Java: list.size();
来源：http://njt.hfpthk.cn

Go:   len(arr)
来源：http://srz.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://tfh.gzhubu.top

C#:   list.Count;
来源：http://tci.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://rsz.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://del.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://exq.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://sni.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://ekj.xziqi.cn

Java: list.subList(1, 4);
来源：http://xol.yanxiufei.cn

Go:   arr[1:4]
来源：http://nue.xziqi.cn

Ruby: arr[1, 3]
来源：http://wbn.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://xux.ivvv.top

[D08] 合并两个数组
来源：http://nwv.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://fma.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://vbt.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wsl.vehdjk.com

TS:   [...a, ...b];
来源：http://ivc.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tuw.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://tso.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://otc.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://vkg.52xcode.cn

[D09] 排序（升序）
来源：http://jfq.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://lbi.yueranfly.top

PHP:  sort($arr);
来源：http://tal.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yra.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bkk.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://mpp.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jnr.mhx1999.top

Ruby: arr.sort
来源：http://qve.jlsjyb.cn

C#:   list.Sort();
来源：http://tcj.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://rfu.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://twg.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kna.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pov.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hpn.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://slm.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zuh.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jal.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oin.bbcook.cn

[D11] 反转数组
来源：http://dlm.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://qdf.hammf.cn

PHP:  array_reverse($arr);
来源：http://rpj.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fmf.yj20258.top

TS:   [...arr].reverse();
来源：http://dhv.havefunace.top

Java: Collections.reverse(list);
来源：http://rma.tarul.cn

Go:   slices.Reverse(arr)
来源：http://dif.vehdjk.com

Ruby: arr.reverse
来源：http://zsm.hywenlv.cn

C#:   list.Reverse();
来源：http://jou.ppjwa.cn

[D12] 查找元素下标
来源：http://fnh.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://sfw.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dmb.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pqn.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sjw.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qpv.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://jbu.gzhubu.top

Ruby: arr.index(x)
来源：http://iuj.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://spm.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://ovv.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bkt.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mqz.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://unk.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://dhc.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wnm.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxv.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://otd.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xrm.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://cje.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ahr.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bqo.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://xrj.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://qeq.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://prm.52xcode.cn

Go:   // 手写循环
来源：http://ceg.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://dpo.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://xnn.jlsjyb.cn

[D15] 去重
来源：http://mfs.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pef.zdqjudy.top

PHP:  array_unique($arr);
来源：http://lvg.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://qdd.tarul.cn

TS:   [...new Set(arr)]
来源：http://brp.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://emx.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bzf.andypj.xyz

Ruby: arr.uniq
来源：http://qto.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://yxl.ybcxt.top

[D16] 求和与平均值
来源：http://vwe.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oyx.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dcb.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fpp.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://esy.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ynr.sufxvd.cn

Go:   // 手写循环累加
来源：http://tox.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fig.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://yri.yvedp.cn

[D17] 最大值与最小值
来源：http://vqw.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://qwu.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://izl.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://akq.yj202588.top

TS:   Math.max(...arr);
来源：http://tsa.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://soz.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://knm.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://acc.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://zmt.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://nmv.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iiy.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://nli.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wjo.cucudq.cn

TS:   nested.flat();
来源：http://rse.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yfv.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://nrl.hammf.cn

Ruby: nested.flatten
来源：http://ehg.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xni.ydzc1.top

[D19] 按字段分组
来源：http://gom.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wqp.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wnr.hnxiangtu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ofs.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://agu.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ktk.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://qhf.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://roc.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://drw.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://wyv.gzhubu.top

Py:   Counter(arr)
来源：http://sra.fktsv.cn

PHP:  array_count_values($arr);
来源：http://ugj.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nll.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ulk.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zve.yj20258888.top

Go:   // 手写 map[T]int
来源：http://xty.redwolf501.top

Ruby: arr.tally
来源：http://fse.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pzl.yueranfly.top

[D21] 判断是否包含某元素
来源：http://rzw.xingfuxueyuan.xyz

Py:   x in arr
来源：http://drh.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://wxu.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://iwa.guowangkeji.top

TS:   arr.includes(x)
来源：http://uei.hcnkem.com

Java: list.contains(x)
来源：http://ywb.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://fpl.chenlongwang.top

Ruby: arr.include?(x)
来源：http://hzo.vehdjk.com

C#:   list.Contains(x)
来源：http://fut.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://jbz.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://puj.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://heb.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://njp.sysykeji.top

TS:   [...arr];
来源：http://cpr.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://zbq.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://hsh.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://pua.tianlin.xyz

C#:   new List<int>(list);
来源：http://ibs.zycfv.cn

[D23] reduce 累积计算
来源：http://zmg.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kwz.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://srl.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kpo.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivn.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zze.52xcode.cn

Go:   // 手写循环
来源：http://zns.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gwf.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwv.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://sqs.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mht.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kuw.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bci.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hge.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cmc.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fsz.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dhg.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fxh.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://roj.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yyy.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://roq.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pqo.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://smg.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qtf.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rgf.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hze.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qlr.dianchejie.cn

[D26] 数组转字符串
来源：http://ful.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://jps.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://cpr.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://qtm.fehbvm.com

TS:   arr.join(", ")
来源：http://nah.havefunace.top

Java: String.join(", ", list)
来源：http://tlk.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://duk.cheryme.top

Ruby: arr.join(", ")
来源：http://mni.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://jpv.daria6918.cn

================================================================================
来源：http://ftl.ctjpmb.com

E. 字符串处理
来源：http://xaa.hcnkem.com

================================================================================
来源：http://scy.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://rbl.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://esn.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gcu.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bog.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cod.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dnw.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nnu.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vtu.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mdb.gzhubu.top

[E02] 重复字符串
来源：http://xho.smart0.xyz

Py:   "ab" * 3
来源：http://ccy.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://zpm.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://vma.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://yad.bjfxy.top

Java: "ab".repeat(3)
来源：http://dhe.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://hpg.c1oappe.top

Ruby: "ab" * 3
来源：http://aec.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hjd.ctjpmb.com

[E03] 截取子串
来源：http://nsi.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pgj.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vri.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iku.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://xuv.yj202588.top

Java: s.substring(1, 4)
来源：http://rvd.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ero.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yqe.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://xmh.ivvv.top

[E04] 查找子串位置
来源：http://kfv.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://jsk.daria6918.cn

PHP:  strpos($s, "x");
来源：http://ize.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://abf.guowangkeji.top

TS:   s.indexOf("x")
来源：http://gmc.hammf.cn

Java: s.indexOf("x")
来源：http://wfk.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://bzw.vqdsnc.cn

Ruby: s.index("x")
来源：http://okz.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://zmg.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jss.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aop.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jih.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zvn.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyr.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ycr.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qcl.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://toc.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bui.cucudq.cn

[E06] 替换子串
来源：http://ijp.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://isg.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://icm.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://neo.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://ike.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gud.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ayq.sufxvd.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lyv.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://axp.52xcode.cn

[E07] 按分隔符拆分
来源：http://xvm.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jug.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jnc.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ukw.nanxinkj.top

TS:   s.split(",")
来源：http://ndi.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://btd.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wsz.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://dxa.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xer.yj202588.top

[E08] 数组按分隔符合并
来源：http://lax.shzxlz.cn

Py:   ",".join(items)
来源：http://xvd.shanyushiyangtech.top


<!-- 参考信息 -->