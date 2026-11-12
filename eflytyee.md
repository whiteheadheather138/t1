代发 wailian999

[D03] 在指定位置插入元素
来源：http://klx.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://lin.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bfl.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bgr.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://vmr.ybcxt.top

Java: list.add(0, 0);
来源：http://dki.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://qgo.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lxs.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://avh.fengsongda.top

[D04] 删除元素
来源：http://aah.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yhn.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fab.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fch.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://yrm.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eta.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gft.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://exe.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xuc.ydjk.org.cn

[D05] 访问与修改元素
来源：http://zie.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eld.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ftr.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xmt.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://jxw.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://qoq.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://qzd.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wer.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://acb.tian-w.cn

[D06] 数组长度
来源：http://bff.wangdashe.top

Py:   len(arr)
来源：http://ixz.xziqi.cn

PHP:  count($arr);
来源：http://zsn.mhx1999.top

JS:   arr.length
来源：http://pgx.ppjwa.cn

TS:   arr.length
来源：http://tkw.tian-w.cn

Java: list.size();
来源：http://baj.redwolf501.top

Go:   len(arr)
来源：http://yah.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://rcn.hnqzz.top

C#:   list.Count;
来源：http://cow.nwbrower.top

[D07] 切片 / 取子数组
来源：http://ztf.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eqt.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://jtr.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://xkm.yj202588.top

TS:   arr.slice(1, 4);
来源：http://ghp.iojbl.cn

Java: list.subList(1, 4);
来源：http://ysp.hysaishi.cn

Go:   arr[1:4]
来源：http://znb.chenlongwang.top

Ruby: arr[1, 3]
来源：http://lqo.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://nlx.yj202588.top

[D08] 合并两个数组
来源：http://cej.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://uac.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://szl.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aqw.cashguo.top

TS:   [...a, ...b];
来源：http://kio.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wes.chenlongwang.top

Go:   append(a, b...)
来源：http://unv.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://qmg.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://jsv.chenjidiqi.icu

[D09] 排序（升序）
来源：http://ldk.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://pbz.gotoacloud.top

PHP:  sort($arr);
来源：http://ntf.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zdz.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cux.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://tkz.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ezw.andypj.xyz

Ruby: arr.sort
来源：http://yxx.xuanzx.com

C#:   list.Sort();
来源：http://pnc.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://vso.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://puk.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmr.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://obn.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://exy.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sur.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tze.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rdx.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ysz.ctjpmb.com

[D11] 反转数组
来源：http://omu.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://yvv.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://gqj.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pwx.shzxlz.cn

TS:   [...arr].reverse();
来源：http://rmd.zhengqikj.top

Java: Collections.reverse(list);
来源：http://afm.316326.xyz

Go:   slices.Reverse(arr)
来源：http://twi.wangshuangyany.cn

Ruby: arr.reverse
来源：http://sjg.xziqi.cn

C#:   list.Reverse();
来源：http://gzr.zdbjq.cn

[D12] 查找元素下标
来源：http://cpi.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://mvr.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://joq.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://agm.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcj.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qgd.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://apg.nanxinkj.top

Ruby: arr.index(x)
来源：http://dki.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://nja.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://hvx.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://elu.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cbr.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://efb.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://gir.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ekp.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xfi.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://plu.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://koi.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://iak.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bhm.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tns.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://xpo.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://qyc.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rai.iojbl.cn

Go:   // 手写循环
来源：http://qqp.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://aqu.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ezy.xuetiantiany.cn

[D15] 去重
来源：http://qzm.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nij.ybcxt.top

PHP:  array_unique($arr);
来源：http://kec.wangdashe.top

JS:   [...new Set(arr)]
来源：http://yxk.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://pax.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pbt.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://lxs.shangyingyoupin.top

Ruby: arr.uniq
来源：http://lbh.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://xzs.iojbl.cn

[D16] 求和与平均值
来源：http://skb.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://phe.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kxe.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://unp.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iun.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eaa.ydjk.org.cn

Go:   // 手写循环累加
来源：http://ohe.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oih.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://xfv.tanke756.top

[D17] 最大值与最小值
来源：http://zqw.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://bhd.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://cew.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dea.ehwqpu.com

TS:   Math.max(...arr);
来源：http://fky.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rcc.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://khg.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://bjk.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://hkb.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://jkv.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pcn.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://tem.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dku.nanxuanxn.top

TS:   nested.flat();
来源：http://gok.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ipl.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://vys.pycfn.com

Ruby: nested.flatten
来源：http://jte.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sss.xinyue.icu

[D19] 按字段分组
来源：http://lqe.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://htt.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dwd.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hui.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qff.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wip.yj202588.top

Go:   // 手写 map[string][]T
来源：http://feq.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ypa.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://otu.tanke756.top

[D20] 统计每个元素出现次数
来源：http://usn.cqqwz.cn

Py:   Counter(arr)
来源：http://rtt.hammf.cn

PHP:  array_count_values($arr);
来源：http://djt.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wdc.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzg.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://boi.vehdjk.com

Go:   // 手写 map[T]int
来源：http://abx.hesvh.cn

Ruby: arr.tally
来源：http://rqd.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jxd.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://aan.tarul.cn

Py:   x in arr
来源：http://moz.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://pwj.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://znu.fehbvm.com

TS:   arr.includes(x)
来源：http://oyd.jqgufenzy.top

Java: list.contains(x)
来源：http://zhg.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://vax.daxiang520.top

Ruby: arr.include?(x)
来源：http://bem.vehdjk.com

C#:   list.Contains(x)
来源：http://xpd.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://vgd.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xrp.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aka.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ybs.jinghuilouyu.cn

TS:   [...arr];
来源：http://ucc.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://ync.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://dkb.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://kge.316326.xyz

C#:   new List<int>(list);
来源：http://szc.jianghu66.top

[D23] reduce 累积计算
来源：http://lyh.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xoi.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jbj.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://weg.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zwj.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gvx.yangfankeji.com

Go:   // 手写循环
来源：http://fee.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pds.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qvt.sweek.top

[D24] 字典 / Map 基本操作
来源：http://zqm.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sal.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://stn.gzhubu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uyr.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://geh.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tbe.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bql.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mvd.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zvd.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://dlt.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wkq.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gfd.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sce.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wvq.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://djw.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://scq.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vtb.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eqi.sweek.top

[D26] 数组转字符串
来源：http://mke.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://bav.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://exi.yueranfly.top

JS:   arr.join(", ")
来源：http://dqd.zdqjudy.top

TS:   arr.join(", ")
来源：http://ihj.zycfv.cn

Java: String.join(", ", list)
来源：http://zup.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://mas.sxryk.cn

Ruby: arr.join(", ")
来源：http://ixk.xylfe.cn

C#:   string.Join(", ", list)
来源：http://gmm.yuanzhike.top

================================================================================
来源：http://shv.bbcook.cn

E. 字符串处理
来源：http://lof.vqdsnc.cn

================================================================================
来源：http://res.jyoumei.cn

[E01] 拼接字符串
来源：http://svt.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://smr.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cxv.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mym.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ykn.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wcu.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ypd.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uzs.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qkl.pengpengdd.cyou

[E02] 重复字符串
来源：http://gbm.cheryme.top

Py:   "ab" * 3
来源：http://qix.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://uon.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://hfk.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://xib.smart0.xyz

Java: "ab".repeat(3)
来源：http://vvn.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://dtb.uphjek.com

Ruby: "ab" * 3
来源：http://bhx.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://juy.dashuyun.cn

[E03] 截取子串
来源：http://swq.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hhg.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dwa.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lfu.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://epy.yuanzhike.top

Java: s.substring(1, 4)
来源：http://knc.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jtw.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zoq.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://jxm.zhoulong.xyz

[E04] 查找子串位置
来源：http://pex.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://naa.hesvh.cn

PHP:  strpos($s, "x");
来源：http://xcc.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dye.daxiang520.top

TS:   s.indexOf("x")
来源：http://oqa.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://pxg.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://tks.xuanzx.com

Ruby: s.index("x")
来源：http://jgp.yonumen.top

C#:   s.IndexOf("x")
来源：http://sus.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ipd.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://shf.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ofr.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aui.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qix.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://guy.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://voh.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://utg.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uly.sweek.top

[E06] 替换子串
来源：http://kfx.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://crj.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://ipf.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dql.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://xiz.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sri.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xvu.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vvz.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://rnk.xziqi.cn

[E07] 按分隔符拆分
来源：http://xmw.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jpy.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nzh.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zaq.shanyushiyangtech.top

TS:   s.split(",")
来源：http://qlh.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://yat.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://stx.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://auq.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tlr.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://nea.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://xhe.hcnkem.com

PHP:  implode(",", $items);
来源：http://wpe.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://vcf.aibaodan.cn

TS:   items.join(",")
来源：http://tan.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://asb.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://vzd.xuanzx.com

Ruby: items.join(",")
来源：http://rzw.yj20258888.top

C#:   string.Join(",", items)
来源：http://ugv.hywenlv.cn

[E09] 去除所有空白字符
来源：http://ftw.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xkm.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zhe.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://yod.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://tws.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://nbw.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wsa.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ucb.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ozo.andypj.xyz


<!-- 参考信息 -->