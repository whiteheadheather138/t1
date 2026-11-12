代发 wailian999

C#:   list.Insert(0, 0);
来源：http://xms.zhaomingkeji.xyz

[D04] 删除元素
来源：http://jsk.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bdq.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://prx.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gxz.tarul.cn

TS:   arr.splice(0, 1);
来源：http://bwb.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pxc.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oau.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hbk.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cid.tanke756.top

[D05] 访问与修改元素
来源：http://tty.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nkc.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rjs.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cwz.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://qqa.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://sha.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://unm.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://adw.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zel.xziqi.cn

[D06] 数组长度
来源：http://gih.0kj1m.cn

Py:   len(arr)
来源：http://bgi.zhengqikj.top

PHP:  count($arr);
来源：http://iwh.zhoulong.xyz

JS:   arr.length
来源：http://cha.iojbl.cn

TS:   arr.length
来源：http://dlu.yueranfly.top

Java: list.size();
来源：http://exi.hnqzz.top

Go:   len(arr)
来源：http://hwq.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://tig.gzhubu.top

C#:   list.Count;
来源：http://cvv.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://zuy.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hgc.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://ovm.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://ick.yongpay.top

TS:   arr.slice(1, 4);
来源：http://syx.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://vue.sysykeji.top

Go:   arr[1:4]
来源：http://tut.ehwqpu.com

Ruby: arr[1, 3]
来源：http://hhj.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://wrw.xinyue.icu

[D08] 合并两个数组
来源：http://ecf.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://wts.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://krk.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://prp.redwolf501.top

TS:   [...a, ...b];
来源：http://axq.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qgl.guannengcc.top

Go:   append(a, b...)
来源：http://wly.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://llr.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://amo.quarkkingdee.top

[D09] 排序（升序）
来源：http://atk.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://ger.haohaochexian.top

PHP:  sort($arr);
来源：http://bat.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rre.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsl.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bso.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://whf.andypj.xyz

Ruby: arr.sort
来源：http://xlk.ehwqpu.com

C#:   list.Sort();
来源：http://dcq.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gbj.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rxw.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xek.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iot.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sxe.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zch.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ptm.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://edz.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dbi.jiagoushi.top

[D11] 反转数组
来源：http://cjg.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://xzq.pycfn.com

PHP:  array_reverse($arr);
来源：http://tve.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wcf.fehbvm.com

TS:   [...arr].reverse();
来源：http://kag.gotoacloud.top

Java: Collections.reverse(list);
来源：http://don.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://zdv.zhixingplan.top

Ruby: arr.reverse
来源：http://rsh.andypj.xyz

C#:   list.Reverse();
来源：http://xoy.haohaochexian.top

[D12] 查找元素下标
来源：http://hsj.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://jnz.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://urt.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rfq.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vst.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vbe.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://pmz.fktsv.cn

Ruby: arr.index(x)
来源：http://mng.mhx1999.top

C#:   list.IndexOf(x);
来源：http://ubd.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://xxa.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://suz.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yor.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://keo.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://hnu.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wav.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xzc.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://ckf.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://agl.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://nwv.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tjb.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://avw.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://pbr.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://zde.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wtg.xziqi.cn

Go:   // 手写循环
来源：http://bkq.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://qnq.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bzr.snrcjt.cn

[D15] 去重
来源：http://nve.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://htx.bjfxy.top

PHP:  array_unique($arr);
来源：http://evc.c1oappe.top

JS:   [...new Set(arr)]
来源：http://dun.shuidangran.top

TS:   [...new Set(arr)]
来源：http://cgk.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://giy.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://bch.vehdjk.com

Ruby: arr.uniq
来源：http://prk.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://rfe.ybcxt.top

[D16] 求和与平均值
来源：http://dgl.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wnf.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ecc.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nng.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xfl.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ugm.shzxlz.cn

Go:   // 手写循环累加
来源：http://hwp.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lwc.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://mfa.hnxiangtu.top

[D17] 最大值与最小值
来源：http://xcn.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://hao.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://iej.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://liw.hesvh.cn

TS:   Math.max(...arr);
来源：http://ims.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ptq.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kqy.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://dav.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://tzb.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://pwq.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rii.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://htt.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aly.yj20258.top

TS:   nested.flat();
来源：http://uiw.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aoz.xuanzx.com

Go:   // 手写双层循环
来源：http://aqk.meibo888.top

Ruby: nested.flatten
来源：http://sol.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rug.bbcook.cn

[D19] 按字段分组
来源：http://abl.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ugd.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zwu.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hck.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://gzj.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://coe.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://rix.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://oac.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ytd.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://pcw.xylfe.cn

Py:   Counter(arr)
来源：http://mht.smart0.xyz

PHP:  array_count_values($arr);
来源：http://dvz.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vpq.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cha.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mbs.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://lnn.havefunace.top

Ruby: arr.tally
来源：http://qie.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oyc.yongpay.top

[D21] 判断是否包含某元素
来源：http://vgf.jinyuanbaomall.cn

Py:   x in arr
来源：http://qyl.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://eye.tarul.cn

JS:   arr.includes(x)
来源：http://afo.chenlongwang.top

TS:   arr.includes(x)
来源：http://nnm.zhengqikj.top

Java: list.contains(x)
来源：http://tlx.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://wmq.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://pun.yj202588.top

C#:   list.Contains(x)
来源：http://ofv.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://ssu.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bfs.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ksw.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xax.zdbjq.cn

TS:   [...arr];
来源：http://mjj.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://kfx.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://bng.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://bwa.gzhubu.top

C#:   new List<int>(list);
来源：http://xjh.ctjpmb.com

[D23] reduce 累积计算
来源：http://zwn.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wnw.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://old.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qtl.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://igt.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mmm.sjlbkw.cn

Go:   // 手写循环
来源：http://vpf.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jni.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rtp.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://ukf.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tfi.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ofe.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://igw.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tvq.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vkl.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kum.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ljh.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aqm.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://izx.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ynh.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://heh.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lts.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kxr.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cac.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qwp.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://poc.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aap.cdnleiting.top

[D26] 数组转字符串
来源：http://zsl.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://xyn.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://svw.quarkkingdee.top

JS:   arr.join(", ")
来源：http://bfn.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://lqp.kuanghao11.cn

Java: String.join(", ", list)
来源：http://cpl.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://xgc.hysaishi.cn

Ruby: arr.join(", ")
来源：http://leq.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://zgb.hammf.cn

================================================================================
来源：http://sjy.jyoumei.cn

E. 字符串处理
来源：http://igb.tianlin.xyz

================================================================================
来源：http://egz.jlsjyb.cn

[E01] 拼接字符串
来源：http://lzx.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qvk.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xeq.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jeb.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ksu.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zwh.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dcq.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xhl.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xzm.jinghuilouyu.cn

[E02] 重复字符串
来源：http://ukp.aibaodan.cn

Py:   "ab" * 3
来源：http://ari.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://rpd.birdmap.top

JS:   "ab".repeat(3)
来源：http://uwm.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://sbf.cucudq.cn

Java: "ab".repeat(3)
来源：http://xsv.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://woi.xylfe.cn

Ruby: "ab" * 3
来源：http://jjc.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wcd.epnwcf.com

[E03] 截取子串
来源：http://ptu.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hud.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cdo.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iob.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://vda.dianchejie.cn

Java: s.substring(1, 4)
来源：http://snh.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://llc.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://lqf.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://klt.gogol.net.cn

[E04] 查找子串位置
来源：http://tpp.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://lkv.havefunace.top

PHP:  strpos($s, "x");
来源：http://zcn.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mws.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://tmh.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://czm.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://vzf.dianchejie.cn

Ruby: s.index("x")
来源：http://zzd.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://xgq.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xfv.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zbr.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eoy.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qfx.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://git.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zrs.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tkj.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://msn.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kfs.yanxiufei.cn

[E06] 替换子串
来源：http://xsj.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bxt.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://wae.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yjp.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://rmg.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fch.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qcw.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ewk.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://glq.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://hwk.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xjl.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://obx.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://huj.tanke756.top

TS:   s.split(",")
来源：http://ljk.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://qiq.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wic.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://uwg.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ymp.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://wnj.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://wld.tanke756.top

PHP:  implode(",", $items);
来源：http://yfu.jqgufenzy.top

JS:   items.join(",")
来源：http://wui.chenlongwang.top

TS:   items.join(",")
来源：http://ree.meibo888.top

Java: String.join(",", items)
来源：http://aec.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://wsa.gzhubu.top

Ruby: items.join(",")
来源：http://aai.tarul.cn

C#:   string.Join(",", items)
来源：http://pmq.yfazqb.com

[E09] 去除所有空白字符
来源：http://dyg.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hnk.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jxo.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://qop.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://zjb.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://ehz.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://nti.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zky.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lyh.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://xbd.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fsg.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ypa.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://mlx.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://czf.uphjek.com

Java: String.format("%03d", 7)
来源：http://uup.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zbj.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tns.dianchejie.cn


<!-- 参考信息 -->