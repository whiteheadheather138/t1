代发 wailian999

Java: list.add(4);
来源：http://kgy.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://bui.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://uwx.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://yvp.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://ais.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://xbx.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vyj.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://apm.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://kbu.xuanzx.com

Java: list.add(0, 0);
来源：http://gor.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rfs.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uov.birdmap.top

C#:   list.Insert(0, 0);
来源：http://qpm.tarul.cn

[D04] 删除元素
来源：http://wpt.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qjl.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uba.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nvs.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://xjg.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rwq.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gua.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gfu.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzv.redwolf501.top

[D05] 访问与修改元素
来源：http://ski.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cbm.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://faj.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qqw.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://clt.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://apb.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://jcg.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bkr.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gok.uphjek.com

[D06] 数组长度
来源：http://vgr.xziqi.cn

Py:   len(arr)
来源：http://uol.hnqzz.top

PHP:  count($arr);
来源：http://apj.jyoumei.cn

JS:   arr.length
来源：http://usn.jlsjyb.cn

TS:   arr.length
来源：http://oee.hongshengwenyu.top

Java: list.size();
来源：http://kld.haohaochexian.top

Go:   len(arr)
来源：http://lfj.daria6918.cn

Ruby: arr.length; arr.size
来源：http://tuf.jianghu66.top

C#:   list.Count;
来源：http://nlp.shuidangran.top

[D07] 切片 / 取子数组
来源：http://vwx.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sre.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wnj.cheryme.top

JS:   arr.slice(1, 4);
来源：http://wrv.hammf.cn

TS:   arr.slice(1, 4);
来源：http://ghj.cucudq.cn

Java: list.subList(1, 4);
来源：http://qnj.cheryme.top

Go:   arr[1:4]
来源：http://fiw.tianlin.xyz

Ruby: arr[1, 3]
来源：http://yxd.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://kte.nanxuanxn.top

[D08] 合并两个数组
来源：http://tfd.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://txj.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://nmz.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xne.aibaodan.cn

TS:   [...a, ...b];
来源：http://umd.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rkz.chenlongwang.top

Go:   append(a, b...)
来源：http://fck.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://nvk.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://bml.guannengcc.top

[D09] 排序（升序）
来源：http://lre.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://swc.jqgfzy.top

PHP:  sort($arr);
来源：http://bes.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://phi.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vrc.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xpn.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ose.yvedp.cn

Ruby: arr.sort
来源：http://vkf.gzhubu.top

C#:   list.Sort();
来源：http://iqi.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kkc.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbm.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ayp.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dll.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvz.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uxd.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xzv.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://szf.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ejc.iojbl.cn

[D11] 反转数组
来源：http://bjn.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://apz.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://hic.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tcb.yuanzhike.top

TS:   [...arr].reverse();
来源：http://tlm.shuidangran.top

Java: Collections.reverse(list);
来源：http://jst.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://dza.hysaishi.cn

Ruby: arr.reverse
来源：http://scp.shzxlz.cn

C#:   list.Reverse();
来源：http://dwg.ctjpmb.com

[D12] 查找元素下标
来源：http://qrf.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://zll.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jzd.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdq.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwx.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wru.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://dsu.fengsongda.top

Ruby: arr.index(x)
来源：http://cpt.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://mxe.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://ftp.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://goo.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pfe.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://vkj.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://mqb.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ifg.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fde.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://yob.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iht.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://ltj.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exq.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pgl.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://npr.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://ico.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://onf.cashguo.top

Go:   // 手写循环
来源：http://ljd.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://orm.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kuk.zhiwuduotai.top

[D15] 去重
来源：http://fek.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ntr.jyoumei.cn

PHP:  array_unique($arr);
来源：http://esh.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://ukn.hammf.cn

TS:   [...new Set(arr)]
来源：http://jmz.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rne.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://bhd.fktsv.cn

Ruby: arr.uniq
来源：http://ovv.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://nmr.hfpthk.cn

[D16] 求和与平均值
来源：http://nhz.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jyq.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://khq.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vcn.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://roj.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vkn.gaohongyu789.top

Go:   // 手写循环累加
来源：http://ksg.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qrg.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://onr.yfazqb.com

[D17] 最大值与最小值
来源：http://qls.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://kae.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://gze.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ouu.hesvh.cn

TS:   Math.max(...arr);
来源：http://nfj.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://wxo.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ddc.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://hwu.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://lbm.sweek.top

[D18] 扁平化嵌套数组
来源：http://pnb.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jrv.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://ngb.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gis.zhixingplan.top

TS:   nested.flat();
来源：http://rvs.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rcj.yongpay.top

Go:   // 手写双层循环
来源：http://bhh.quarkkingdee.top

Ruby: nested.flatten
来源：http://avt.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://age.jinqigfzy.top

[D19] 按字段分组
来源：http://vki.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hqn.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nxi.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qqx.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ibb.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aed.ivvv.top

Go:   // 手写 map[string][]T
来源：http://kid.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iog.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dmc.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://ufr.feifeiyinyue.top

Py:   Counter(arr)
来源：http://qwc.uphjek.com

PHP:  array_count_values($arr);
来源：http://egr.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vzq.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qgw.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fbf.wangdashe.top

Go:   // 手写 map[T]int
来源：http://yiy.aizwys.cn

Ruby: arr.tally
来源：http://abw.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sii.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://bih.snrcjt.cn

Py:   x in arr
来源：http://hro.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://aov.yongpay.top

JS:   arr.includes(x)
来源：http://dov.aibaodan.cn

TS:   arr.includes(x)
来源：http://kcm.dianchejie.cn

Java: list.contains(x)
来源：http://ags.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://stm.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://eyi.chenzaomai.com

C#:   list.Contains(x)
来源：http://lox.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://aqk.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://exu.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://suv.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vjx.jlsjyb.cn

TS:   [...arr];
来源：http://xiy.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://mek.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://fcw.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://jyn.bjfxy.top

C#:   new List<int>(list);
来源：http://wfy.yonumen.top

[D23] reduce 累积计算
来源：http://ffh.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lqq.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vyf.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wai.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pkn.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kpj.316326.xyz

Go:   // 手写循环
来源：http://uvj.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zfd.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iwv.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://cmp.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://owo.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mji.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jhd.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://djx.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://evv.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zqj.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ieo.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hyl.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://icy.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lvs.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tbd.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dmj.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qef.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://apo.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nbb.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bbw.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hpq.tian-w.cn

[D26] 数组转字符串
来源：http://rmi.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://baz.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://lum.yuxming.cn

JS:   arr.join(", ")
来源：http://ydw.uphjek.com

TS:   arr.join(", ")
来源：http://hfn.jqgufenzy.top

Java: String.join(", ", list)
来源：http://ooo.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://rcz.zycfv.cn

Ruby: arr.join(", ")
来源：http://xmj.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://jbi.nwbrower.top

================================================================================
来源：http://cck.shzxlz.cn

E. 字符串处理
来源：http://fye.yj202588.top

================================================================================
来源：http://ikv.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://jhz.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yfi.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xsu.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zsf.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://anx.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ztf.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gzx.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://itg.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uvb.epnwcf.com

[E02] 重复字符串
来源：http://uwc.redwolf501.top

Py:   "ab" * 3
来源：http://vxs.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://tzj.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://fbu.aizwys.cn

TS:   "ab".repeat(3)
来源：http://jef.cdnleiting.top

Java: "ab".repeat(3)
来源：http://xru.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://uin.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://wyv.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jap.fanxiaobao.xyz

[E03] 截取子串
来源：http://dnw.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gyz.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hbb.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rbj.daxiang520.top

TS:   s.slice(1, 4)
来源：http://apw.hammf.cn

Java: s.substring(1, 4)
来源：http://jmz.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bzy.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://rxg.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://zrv.52xcode.cn

[E04] 查找子串位置
来源：http://arp.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://kbo.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://bmo.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://myc.ivvv.top

TS:   s.indexOf("x")
来源：http://rot.chenlongwang.top

Java: s.indexOf("x")
来源：http://iea.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://ten.cucudq.cn

Ruby: s.index("x")
来源：http://qtg.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://gsp.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ifc.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rxt.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nxa.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxy.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kna.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hwo.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hpq.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvv.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nnt.guowangkeji.top

[E06] 替换子串
来源：http://zef.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vnb.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://dwr.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jad.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://nbb.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jst.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oce.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yll.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://cks.tian-w.cn

[E07] 按分隔符拆分
来源：http://uxr.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xvz.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uzo.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cld.hongshengwenyu.top

TS:   s.split(",")
来源：http://ivc.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://kdr.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://stj.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://xvy.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bew.52xcode.cn

[E08] 数组按分隔符合并
来源：http://zkh.aibaodan.cn

Py:   ",".join(items)
来源：http://zer.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://efa.pycfn.com

JS:   items.join(",")
来源：http://dug.ppjwa.cn

TS:   items.join(",")
来源：http://hdh.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://jhl.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://ozt.yj20258.top

Ruby: items.join(",")
来源：http://lpk.cucudq.cn

C#:   string.Join(",", items)
来源：http://ffm.fengsongda.top

[E09] 去除所有空白字符
来源：http://hbx.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mzw.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aqo.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://tkf.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://oyo.jqgufenzy.top


<!-- 参考信息 -->