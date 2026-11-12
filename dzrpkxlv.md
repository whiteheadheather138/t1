代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://gpt.sufxvd.cn

Java: list.add(0, 0);
来源：http://bqx.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dzl.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://llh.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://auc.jinghuilouyu.cn

[D04] 删除元素
来源：http://eet.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kkd.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ghw.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kuy.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://mir.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uxu.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fyz.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ifd.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wzs.yvedp.cn

[D05] 访问与修改元素
来源：http://bzg.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://abm.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fgy.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://spq.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://ont.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://lgh.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://tap.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oys.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ifq.ehwqpu.com

[D06] 数组长度
来源：http://jvw.fzhhl.top

Py:   len(arr)
来源：http://yrw.chenlongwang.top

PHP:  count($arr);
来源：http://zos.chenlongwang.top

JS:   arr.length
来源：http://ppl.havefunace.top

TS:   arr.length
来源：http://aax.yuanzhike.top

Java: list.size();
来源：http://sya.sjlbkw.cn

Go:   len(arr)
来源：http://qho.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://hue.quarkkingdee.top

C#:   list.Count;
来源：http://ueh.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://uji.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ouw.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xgd.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://kws.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://lva.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://mqu.guowangkeji.top

Go:   arr[1:4]
来源：http://uip.smart0.xyz

Ruby: arr[1, 3]
来源：http://bsi.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://krc.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://wiy.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://ewt.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://smx.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hbu.tianlin.xyz

TS:   [...a, ...b];
来源：http://cff.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iwc.yuanzhike.top

Go:   append(a, b...)
来源：http://pvt.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://oyc.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://uia.sufxvd.cn

[D09] 排序（升序）
来源：http://zfr.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://fxb.jqgufenzy.top

PHP:  sort($arr);
来源：http://tku.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wxa.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xke.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lss.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vwb.c1oappe.top

Ruby: arr.sort
来源：http://ljb.guannengcc.top

C#:   list.Sort();
来源：http://rgk.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qyg.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xue.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oro.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jho.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ipw.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://szx.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xia.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://utu.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xtf.cqqwz.cn

[D11] 反转数组
来源：http://qfe.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ykz.zycfv.cn

PHP:  array_reverse($arr);
来源：http://ihs.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zru.ivvv.top

TS:   [...arr].reverse();
来源：http://zqt.gzhubu.top

Java: Collections.reverse(list);
来源：http://wxe.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://abi.sjlbkw.cn

Ruby: arr.reverse
来源：http://asz.shuidangran.top

C#:   list.Reverse();
来源：http://dwx.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://emx.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://tgu.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ivb.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tqd.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ajx.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iui.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://hbl.daxiang520.top

Ruby: arr.index(x)
来源：http://xji.xinyue.icu

C#:   list.IndexOf(x);
来源：http://pmp.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://uvm.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://plp.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ghc.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://hgy.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://dhj.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cuv.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lia.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://xxx.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tnk.epnwcf.com

[D14] 映射转换（每个元素变形）
来源：http://rab.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lri.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zwm.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://qle.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://oen.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwx.shuidangran.top

Go:   // 手写循环
来源：http://rhf.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://mze.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cuy.sysykeji.top

[D15] 去重
来源：http://vax.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nkg.jianghu66.top

PHP:  array_unique($arr);
来源：http://lfl.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://yxh.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://wcx.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tri.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://rtl.xziqi.cn

Ruby: arr.uniq
来源：http://uoc.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://qxt.vehdjk.com

[D16] 求和与平均值
来源：http://adj.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qut.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jge.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ljf.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://shm.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hjs.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://gbn.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xtj.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://scx.shzxlz.cn

[D17] 最大值与最小值
来源：http://wat.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://trl.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://gaw.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tai.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://iik.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ecn.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mww.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://ooe.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://nya.yonumen.top

[D18] 扁平化嵌套数组
来源：http://ufz.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dnx.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://etp.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tqe.tianlin.xyz

TS:   nested.flat();
来源：http://ful.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rpm.bjfxy.top

Go:   // 手写双层循环
来源：http://atm.tanke756.top

Ruby: nested.flatten
来源：http://wmr.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://cvm.shuidangran.top

[D19] 按字段分组
来源：http://zxk.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qol.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ggr.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hds.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pkk.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xcj.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://tzj.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oxc.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xdp.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://jmf.hnqzz.top

Py:   Counter(arr)
来源：http://yew.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://xkb.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sig.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hgv.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kmi.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://bja.zhiwuduotai.top

Ruby: arr.tally
来源：http://lqj.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfx.sysykeji.top

[D21] 判断是否包含某元素
来源：http://gcj.yfazqb.com

Py:   x in arr
来源：http://ysk.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://tlz.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://cpd.yuanzhike.top

TS:   arr.includes(x)
来源：http://xpt.cdnleiting.top

Java: list.contains(x)
来源：http://zkw.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://jim.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://vrw.guannengcc.top

C#:   list.Contains(x)
来源：http://adi.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://iyd.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dbt.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aic.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lku.yongpay.top

TS:   [...arr];
来源：http://ipc.ivvv.top

Java: new ArrayList<>(list);
来源：http://ytw.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://apm.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://scu.chenlongwang.top

C#:   new List<int>(list);
来源：http://lig.zdqjudy.top

[D23] reduce 累积计算
来源：http://sdd.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vqf.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ubr.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ujd.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qff.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://exm.jlsjyb.cn

Go:   // 手写循环
来源：http://hqr.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iow.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yma.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://dzn.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://izw.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cid.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jce.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jmk.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ttg.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jhk.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gfc.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xnm.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://xqf.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nnx.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bvs.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hdt.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kwl.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://grj.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jdt.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jye.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nmm.feifeiyinyue.top

[D26] 数组转字符串
来源：http://vsc.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://oml.316326.xyz

PHP:  implode(", ", $arr);
来源：http://uim.shuidangran.top

JS:   arr.join(", ")
来源：http://bef.hysaishi.cn

TS:   arr.join(", ")
来源：http://oxk.gaohongyu789.top

Java: String.join(", ", list)
来源：http://tzn.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://roi.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://fqp.fzhhl.top

C#:   string.Join(", ", list)
来源：http://gyp.aibaodan.cn

================================================================================
来源：http://dmg.hysaishi.cn

E. 字符串处理
来源：http://ssm.zdbjq.cn

================================================================================
来源：http://mmp.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://yat.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fyb.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wnk.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iee.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://itw.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zms.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ghn.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vud.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lun.ppjwa.cn

[E02] 重复字符串
来源：http://dky.wangshuangyany.cn

Py:   "ab" * 3
来源：http://ybe.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://elz.aizwys.cn

JS:   "ab".repeat(3)
来源：http://pgf.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://ydg.yj202588.top

Java: "ab".repeat(3)
来源：http://uzf.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://rxp.yonumen.top

Ruby: "ab" * 3
来源：http://rhe.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mlb.xylfe.cn

[E03] 截取子串
来源：http://jae.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eqp.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uoa.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lby.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://nzx.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://rgl.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sbs.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://iie.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://ovp.cdnleiting.top

[E04] 查找子串位置
来源：http://jtg.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://wxv.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://xcn.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tzw.meibo888.top

TS:   s.indexOf("x")
来源：http://plh.pengpengdd.cyou

Java: s.indexOf("x")
来源：http://gxk.uphjek.com

Go:   strings.Index(s, "x")
来源：http://peb.bbcook.cn

Ruby: s.index("x")
来源：http://mib.havefunace.top

C#:   s.IndexOf("x")
来源：http://rrh.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dws.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qtr.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://chd.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://exz.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uzn.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iaz.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qsq.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://odv.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wev.shangyingyoupin.top

[E06] 替换子串
来源：http://jft.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rkf.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://cuf.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oko.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://tpz.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aph.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iqq.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lbr.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://shd.hcnkem.com

[E07] 按分隔符拆分
来源：http://wjz.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aox.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mpa.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wlu.kuanghao11.cn

TS:   s.split(",")
来源：http://zlx.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://bly.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nvj.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://qrh.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://whq.ivvv.top

[E08] 数组按分隔符合并
来源：http://gxi.meibo888.top

Py:   ",".join(items)
来源：http://lyz.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://fwj.jqgfzy.top

JS:   items.join(",")
来源：http://pfn.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://vej.hysaishi.cn

Java: String.join(",", items)
来源：http://byh.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://igs.xuanzx.com

Ruby: items.join(",")
来源：http://evp.iojbl.cn

C#:   string.Join(",", items)
来源：http://czm.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://skc.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qth.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dcg.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://uji.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://ojy.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://ivx.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pyn.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gwj.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ejc.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://lyl.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uqz.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tgh.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://wir.ydjk.org.cn


<!-- 参考信息 -->