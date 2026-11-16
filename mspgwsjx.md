代发 wailian999

C#:   list.Insert(0, 0);
来源：http://tbe.haohaochexian.top

[D04] 删除元素
来源：http://qpy.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dod.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rtm.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mev.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://vgl.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xlm.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dka.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vme.yangfankeji.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bwd.ppjwa.cn

[D05] 访问与修改元素
来源：http://xdc.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jnw.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ood.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dfz.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://rqm.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://oyx.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://rmk.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xqm.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cek.0kj1m.cn

[D06] 数组长度
来源：http://pqh.52xcode.cn

Py:   len(arr)
来源：http://hom.jianghu66.top

PHP:  count($arr);
来源：http://phk.feifeiyinyue.top

JS:   arr.length
来源：http://zrk.pengpengdd.cyou

TS:   arr.length
来源：http://qva.shuidangran.top

Java: list.size();
来源：http://dgj.0kj1m.cn

Go:   len(arr)
来源：http://tok.birdmap.top

Ruby: arr.length; arr.size
来源：http://vqe.yj202588.top

C#:   list.Count;
来源：http://ftr.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://ewe.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ang.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://jcw.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://ggp.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://tza.fehbvm.com

Java: list.subList(1, 4);
来源：http://ehd.52xcode.cn

Go:   arr[1:4]
来源：http://jhu.hysaishi.cn

Ruby: arr[1, 3]
来源：http://wmi.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://lou.svipenyu.cn

[D08] 合并两个数组
来源：http://jts.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://bmz.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://ofn.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jxj.svipenyu.cn

TS:   [...a, ...b];
来源：http://vjd.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rxc.havefunace.top

Go:   append(a, b...)
来源：http://vki.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://fyt.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://wey.ybcxt.top

[D09] 排序（升序）
来源：http://gdm.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://lki.chenzaomai.com

PHP:  sort($arr);
来源：http://pzx.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mqa.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kpo.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hmc.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dvb.yangfankeji.com

Ruby: arr.sort
来源：http://tdl.gotoacloud.top

C#:   list.Sort();
来源：http://czm.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hsr.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mze.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://slp.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwk.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vmu.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mwg.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wrf.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqi.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dlg.daxiang520.top

[D11] 反转数组
来源：http://drr.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://rlr.yj20258888.top

PHP:  array_reverse($arr);
来源：http://sca.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hvx.yj20258.top

TS:   [...arr].reverse();
来源：http://kaq.meibo888.top

Java: Collections.reverse(list);
来源：http://gds.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://vjp.yueranfly.top

Ruby: arr.reverse
来源：http://tqx.ybcxt.top

C#:   list.Reverse();
来源：http://mpe.yueranfly.top

[D12] 查找元素下标
来源：http://upk.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://sjg.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://htl.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mgm.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vgi.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mbv.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://pir.ctjpmb.com

Ruby: arr.index(x)
来源：http://wzl.vehdjk.com

C#:   list.IndexOf(x);
来源：http://msc.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://aup.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vnd.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qgo.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://lkh.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://gjt.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zgz.yuxming.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iiu.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wqe.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kgu.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://lfu.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zeq.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rlx.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://asi.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://gtn.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pyb.jiagoushi.top

Go:   // 手写循环
来源：http://trs.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ach.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pvm.pycfn.com

[D15] 去重
来源：http://qao.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pyb.yvedp.cn

PHP:  array_unique($arr);
来源：http://xok.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://vzt.ybcxt.top

TS:   [...new Set(arr)]
来源：http://mcm.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yye.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ocp.haohaochexian.top

Ruby: arr.uniq
来源：http://gdb.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://uat.sufxvd.cn

[D16] 求和与平均值
来源：http://bnu.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://quc.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zvs.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://job.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xeu.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vxw.cqqwz.cn

Go:   // 手写循环累加
来源：http://wmu.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emm.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://vzu.jqgfzy.top

[D17] 最大值与最小值
来源：http://jgz.meibo888.top

Py:   max(arr);  min(arr)
来源：http://mih.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://ead.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxo.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://ysm.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kmo.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gvn.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://rrk.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://qqp.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://dkd.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ble.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://aox.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rqx.jyoumei.cn

TS:   nested.flat();
来源：http://szh.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zlz.yonumen.top

Go:   // 手写双层循环
来源：http://zmt.nwbrower.top

Ruby: nested.flatten
来源：http://ldm.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nhc.guannengcc.top

[D19] 按字段分组
来源：http://zza.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fpp.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ixb.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fyw.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bkq.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fhg.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://ica.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nte.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mny.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://udl.aibaodan.cn

Py:   Counter(arr)
来源：http://lud.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://wvj.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cgz.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://opo.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bad.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://dig.bjfxy.top

Ruby: arr.tally
来源：http://obp.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wpj.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://smx.ehwqpu.com

Py:   x in arr
来源：http://ebk.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://xzn.zhongyouzk.top

JS:   arr.includes(x)
来源：http://vcw.mhx1999.top

TS:   arr.includes(x)
来源：http://wfe.jinghuilouyu.cn

Java: list.contains(x)
来源：http://gqi.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://pkb.gogol.net.cn

Ruby: arr.include?(x)
来源：http://ylj.hesvh.cn

C#:   list.Contains(x)
来源：http://nnl.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://hkf.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fhf.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ejv.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ine.zhijiandao.cn

TS:   [...arr];
来源：http://hnu.fktsv.cn

Java: new ArrayList<>(list);
来源：http://gre.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jsg.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://ths.shuidangran.top

C#:   new List<int>(list);
来源：http://ofg.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://him.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tqj.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wmr.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nve.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://btv.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kab.jqgufenzy.top

Go:   // 手写循环
来源：http://gzm.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wdg.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nym.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://otp.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gbd.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gsu.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://znn.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gtz.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xvd.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fyp.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xwp.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uuf.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://evp.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gzu.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://orv.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://edz.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kvx.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iwo.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lio.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xhe.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tmy.yuanzhike.top

[D26] 数组转字符串
来源：http://jag.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://ttx.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://edg.cashguo.top

JS:   arr.join(", ")
来源：http://jsd.epnwcf.com

TS:   arr.join(", ")
来源：http://wqo.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://egp.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://tpz.jqgfzy.top

Ruby: arr.join(", ")
来源：http://ojk.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://ldn.shanyushiyangkeji.top

================================================================================
来源：http://svd.jianghu66.top

E. 字符串处理
来源：http://lwi.zhengqikj.top

================================================================================
来源：http://riy.havefunace.top

[E01] 拼接字符串
来源：http://oab.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qba.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iot.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ity.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pqk.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jyk.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cgv.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://okw.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://trx.jyoumei.cn

[E02] 重复字符串
来源：http://bth.bbcook.cn

Py:   "ab" * 3
来源：http://uzg.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://uuf.fehbvm.com

JS:   "ab".repeat(3)
来源：http://hwb.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://vlf.xziqi.cn

Java: "ab".repeat(3)
来源：http://wwl.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://err.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://pbw.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yux.uphjek.com

[E03] 截取子串
来源：http://szu.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jtp.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zpv.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ppl.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://kqf.0kj1m.cn

Java: s.substring(1, 4)
来源：http://tax.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wpp.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://vno.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://qmr.52xcode.cn

[E04] 查找子串位置
来源：http://iin.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://dzi.yj20258.top

PHP:  strpos($s, "x");
来源：http://zxy.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fex.aizwys.cn

TS:   s.indexOf("x")
来源：http://llp.snrcjt.cn

Java: s.indexOf("x")
来源：http://ytt.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://cfv.chenjidiqi.icu

Ruby: s.index("x")
来源：http://tzw.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://eyg.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ibq.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cbp.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kcf.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dbv.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cay.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tyl.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://doe.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ohw.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tis.xinyue.icu

[E06] 替换子串
来源：http://aft.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgk.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://tkg.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xai.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://mdj.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aue.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vla.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sax.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://nox.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://ybe.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hyb.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lpc.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hoz.fanxiaobao.xyz

TS:   s.split(",")
来源：http://bgp.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://cif.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dcu.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://wse.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cwk.c1oappe.top

[E08] 数组按分隔符合并
来源：http://dxp.yvedp.cn

Py:   ",".join(items)
来源：http://swb.cashguo.top

PHP:  implode(",", $items);
来源：http://vgg.yj20258888.top

JS:   items.join(",")
来源：http://eil.ehwqpu.com

TS:   items.join(",")
来源：http://rib.hfpthk.cn

Java: String.join(",", items)
来源：http://ztc.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://fey.hammf.cn

Ruby: items.join(",")
来源：http://fgn.dashuyun.cn

C#:   string.Join(",", items)
来源：http://ydl.yuxming.cn

[E09] 去除所有空白字符
来源：http://qon.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://moj.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pzi.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://pog.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://odg.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://roe.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pbn.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://awj.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fqc.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://svq.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qvx.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://krq.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://uyw.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://thk.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://tqo.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vgi.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://opb.mhx1999.top


<!-- 参考信息 -->