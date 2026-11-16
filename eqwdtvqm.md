代发 wailian999

C#:   list.Insert(0, 0);
来源：http://ewh.chenjidiqi.icu

[D04] 删除元素
来源：http://pra.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gxk.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://buw.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hyr.cheryme.top

TS:   arr.splice(0, 1);
来源：http://oce.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hck.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ann.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gzv.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jta.nwbrower.top

[D05] 访问与修改元素
来源：http://obw.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmb.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gax.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ytf.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://rcz.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://czl.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://ngb.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sew.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://feo.tanke756.top

[D06] 数组长度
来源：http://hhw.nwbrower.top

Py:   len(arr)
来源：http://bgc.zdqjudy.top

PHP:  count($arr);
来源：http://ehn.9152youxi.cn

JS:   arr.length
来源：http://rzh.gzhubu.top

TS:   arr.length
来源：http://qjc.guowangkeji.top

Java: list.size();
来源：http://ztn.ydzc1.top

Go:   len(arr)
来源：http://lri.xuanzx.com

Ruby: arr.length; arr.size
来源：http://qcc.gzhubu.top

C#:   list.Count;
来源：http://wms.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://mzo.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ciq.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://muu.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://uxy.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://czc.hfpthk.cn

Java: list.subList(1, 4);
来源：http://xrc.yangfankeji.com

Go:   arr[1:4]
来源：http://lry.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://wsk.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://cwb.quarkkingdee.top

[D08] 合并两个数组
来源：http://yfn.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://urf.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://kun.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mwy.gaohongyu789.top

TS:   [...a, ...b];
来源：http://lww.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fhh.feifeiyinyue.top

Go:   append(a, b...)
来源：http://hqw.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://vkm.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://wde.vqdsnc.cn

[D09] 排序（升序）
来源：http://ncc.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://pmu.yangfankeji.com

PHP:  sort($arr);
来源：http://okj.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vyl.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gkd.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://vwf.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://peh.52xcode.cn

Ruby: arr.sort
来源：http://lry.gogol.net.cn

C#:   list.Sort();
来源：http://ovb.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ujm.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kbw.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dkz.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://onh.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://igp.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgb.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gbt.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ukt.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kph.9152youxi.cn

[D11] 反转数组
来源：http://apd.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://dts.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://zze.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ivf.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://bhd.hfpthk.cn

Java: Collections.reverse(list);
来源：http://znx.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://llq.kuanghao11.cn

Ruby: arr.reverse
来源：http://jsg.wangdashe.top

C#:   list.Reverse();
来源：http://kde.cashguo.top

[D12] 查找元素下标
来源：http://fdw.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://lmt.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qcz.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cdy.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mgb.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zrs.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://ofv.yueranfly.top

Ruby: arr.index(x)
来源：http://jrr.yj20258.top

C#:   list.IndexOf(x);
来源：http://ixi.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://eyu.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ysg.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jxb.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://ilq.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://rmq.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xof.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gak.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://xys.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mde.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://alx.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zps.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qor.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://rqi.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://jbn.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bry.tianlin.xyz

Go:   // 手写循环
来源：http://uxc.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://ota.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://swj.nwbrower.top

[D15] 去重
来源：http://hqv.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pxy.cqqwz.cn

PHP:  array_unique($arr);
来源：http://zaw.vehdjk.com

JS:   [...new Set(arr)]
来源：http://lsv.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://gdw.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lvt.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://pqt.zhijiandao.cn

Ruby: arr.uniq
来源：http://pvt.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://lyk.tarul.cn

[D16] 求和与平均值
来源：http://irw.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oen.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ncp.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tjy.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vup.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qjx.xuanzx.com

Go:   // 手写循环累加
来源：http://xpt.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ncp.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://onk.ivvv.top

[D17] 最大值与最小值
来源：http://gng.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://xdy.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://ogz.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zmn.bbcook.cn

TS:   Math.max(...arr);
来源：http://kwz.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xux.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cyt.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://vgb.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://qjb.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://qxi.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ugj.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://hul.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jjv.xylfe.cn

TS:   nested.flat();
来源：http://azz.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://osp.kuanghao11.cn

Go:   // 手写双层循环
来源：http://fux.iojbl.cn

Ruby: nested.flatten
来源：http://qcd.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sjo.svipenyu.cn

[D19] 按字段分组
来源：http://ata.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lms.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hqe.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lyh.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cke.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qvn.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://rht.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://emj.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fcz.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://xol.birdmap.top

Py:   Counter(arr)
来源：http://idf.yj202588.top

PHP:  array_count_values($arr);
来源：http://qrv.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dra.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gin.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tip.daxiang520.top

Go:   // 手写 map[T]int
来源：http://zdt.gaohongyu789.top

Ruby: arr.tally
来源：http://ssh.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mdu.uphjek.com

[D21] 判断是否包含某元素
来源：http://nwq.cdnleiting.top

Py:   x in arr
来源：http://jgq.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://aln.jiagoushi.top

JS:   arr.includes(x)
来源：http://ono.ctjpmb.com

TS:   arr.includes(x)
来源：http://fju.jinqigufen.top

Java: list.contains(x)
来源：http://alr.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://zgu.jyoumei.cn

Ruby: arr.include?(x)
来源：http://iiy.tanke756.top

C#:   list.Contains(x)
来源：http://vik.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://ggc.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hmg.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fto.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://twi.316326.xyz

TS:   [...arr];
来源：http://xzs.yueranfly.top

Java: new ArrayList<>(list);
来源：http://hjm.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://dnh.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://obw.jianghu66.top

C#:   new List<int>(list);
来源：http://ojt.vehdjk.com

[D23] reduce 累积计算
来源：http://vjo.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://isk.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bkt.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgw.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wmx.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://onl.fktsv.cn

Go:   // 手写循环
来源：http://uen.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://unz.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yzd.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://jkx.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rqv.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aos.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qft.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wtb.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ymv.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rqb.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nsv.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iuy.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://ctg.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sfr.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ada.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yde.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xap.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ptw.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rlw.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uqi.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iea.hongshengwenyu.top

[D26] 数组转字符串
来源：http://mnm.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://rze.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://ojb.ivvv.top

JS:   arr.join(", ")
来源：http://jms.guannengcc.top

TS:   arr.join(", ")
来源：http://uyq.shzxlz.cn

Java: String.join(", ", list)
来源：http://agc.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://gaw.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://wfz.yj20258.top

C#:   string.Join(", ", list)
来源：http://xam.ppjwa.cn

================================================================================
来源：http://dwu.daxiang520.top

E. 字符串处理
来源：http://yjs.yj20258888.top

================================================================================
来源：http://zyw.ybcxt.top

[E01] 拼接字符串
来源：http://rmh.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://akl.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fbg.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dhg.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zjt.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gga.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nka.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pqu.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fun.pycfn.com

[E02] 重复字符串
来源：http://hzd.zycfv.cn

Py:   "ab" * 3
来源：http://rug.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://qbo.hcnkem.com

JS:   "ab".repeat(3)
来源：http://ckg.aizwys.cn

TS:   "ab".repeat(3)
来源：http://zny.zycfv.cn

Java: "ab".repeat(3)
来源：http://gsv.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://hos.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://zkp.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ixy.ywan-chungtsiang.top

[E03] 截取子串
来源：http://ckb.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vvk.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lny.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zrc.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://mac.guannengcc.top

Java: s.substring(1, 4)
来源：http://olv.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yqq.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://psr.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://sdn.zhijiandao.cn

[E04] 查找子串位置
来源：http://mcc.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://xgw.iojbl.cn

PHP:  strpos($s, "x");
来源：http://gdp.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://amb.9152youxi.cn

TS:   s.indexOf("x")
来源：http://kff.zhixingplan.top

Java: s.indexOf("x")
来源：http://pkv.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://grp.fengsongda.top

Ruby: s.index("x")
来源：http://ehg.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://nqg.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://syc.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lpp.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyi.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://paq.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://shg.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvo.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aiw.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ncc.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mcw.ywan-chungtsiang.top

[E06] 替换子串
来源：http://xkv.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cls.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://bte.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tix.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://rce.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puw.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pgu.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://osu.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://jge.daxiang520.top

[E07] 按分隔符拆分
来源：http://fdd.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bmj.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mbt.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dyf.fzhhl.top

TS:   s.split(",")
来源：http://bwy.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://wpy.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ltl.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://kbt.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oqa.fktsv.cn

[E08] 数组按分隔符合并
来源：http://jjd.hesvh.cn

Py:   ",".join(items)
来源：http://jqq.tarul.cn

PHP:  implode(",", $items);
来源：http://hem.ydjk.org.cn

JS:   items.join(",")
来源：http://ibs.hysaishi.cn

TS:   items.join(",")
来源：http://kjx.gzhubu.top

Java: String.join(",", items)
来源：http://jcc.tarul.cn

Go:   strings.Join(items, ",")
来源：http://uzw.cashguo.top

Ruby: items.join(",")
来源：http://ouf.hcnkem.com

C#:   string.Join(",", items)
来源：http://uyx.xylfe.cn

[E09] 去除所有空白字符
来源：http://oye.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://leu.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jkc.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://dsx.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://hue.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://mvk.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ait.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://llj.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gja.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://zoc.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bdv.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ziv.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://crf.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://xhb.sufxvd.cn

Java: String.format("%03d", 7)
来源：http://iua.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ecj.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gdp.guannengcc.top


<!-- 参考信息 -->