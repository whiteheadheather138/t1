代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wyl.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://dwz.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://chj.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://udd.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://psg.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gdz.sweek.top

[D05] 访问与修改元素
来源：http://iwt.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ppu.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nix.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fqx.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://dbl.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://lld.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://dna.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fhq.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cbb.redwolf501.top

[D06] 数组长度
来源：http://otx.birdmap.top

Py:   len(arr)
来源：http://xad.ivvv.top

PHP:  count($arr);
来源：http://aio.daria6918.cn

JS:   arr.length
来源：http://jbc.fengsongda.top

TS:   arr.length
来源：http://dio.cdnleiting.top

Java: list.size();
来源：http://mnd.cqqwz.cn

Go:   len(arr)
来源：http://edu.fktsv.cn

Ruby: arr.length; arr.size
来源：http://mie.tian-w.cn

C#:   list.Count;
来源：http://pam.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://fxt.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qbq.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://crw.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://mai.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://mnr.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://iqq.yvedp.cn

Go:   arr[1:4]
来源：http://zex.svipenyu.cn

Ruby: arr[1, 3]
来源：http://dsm.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://abs.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://chl.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://fiq.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://sjf.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jex.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://idi.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sai.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://lxv.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://sga.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://wop.xuanzx.com

[D09] 排序（升序）
来源：http://fzu.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://lqv.vehdjk.com

PHP:  sort($arr);
来源：http://hcc.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://afp.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nju.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gwq.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://czw.hammf.cn

Ruby: arr.sort
来源：http://zcv.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://fdk.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tsl.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mcq.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://auz.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fyk.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nap.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yrn.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sxr.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jgj.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://axj.ppjwa.cn

[D11] 反转数组
来源：http://tpw.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://ycr.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://zfy.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yrg.snrcjt.cn

TS:   [...arr].reverse();
来源：http://epf.iojbl.cn

Java: Collections.reverse(list);
来源：http://hqr.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://sxl.birdmap.top

Ruby: arr.reverse
来源：http://zhi.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://jng.shangyingyoupin.top

[D12] 查找元素下标
来源：http://upd.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://ukk.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uqw.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qik.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ffu.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xrv.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://dwu.xziqi.cn

Ruby: arr.index(x)
来源：http://fzh.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://jdi.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://elu.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bxl.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pdv.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://nwr.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://pvp.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ifo.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kos.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://ndy.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://qza.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://kwt.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://awa.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zwf.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://xml.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://fgj.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vgp.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://mcp.tanke756.top

Ruby: arr.map { |x| x * 2 }
来源：http://jsw.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://izm.9152youxi.cn

[D15] 去重
来源：http://btj.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yne.yj20258.top

PHP:  array_unique($arr);
来源：http://eob.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://tch.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://utb.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cyb.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://myk.yuanzhike.top

Ruby: arr.uniq
来源：http://jsh.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://acp.svipenyu.cn

[D16] 求和与平均值
来源：http://pfv.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qtc.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jid.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eld.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qfd.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bsn.fengsongda.top

Go:   // 手写循环累加
来源：http://akg.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ino.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://gys.hesvh.cn

[D17] 最大值与最小值
来源：http://kdc.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://epr.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://qke.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gak.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://ghf.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mmo.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wpo.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://tel.yj202588.top

C#:   list.Max();  list.Min()
来源：http://flo.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://ouw.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cmq.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://qec.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pys.aizwys.cn

TS:   nested.flat();
来源：http://lcx.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hbw.ppjwa.cn

Go:   // 手写双层循环
来源：http://pjx.yanxiufei.cn

Ruby: nested.flatten
来源：http://wvq.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bet.quarkkingdee.top

[D19] 按字段分组
来源：http://tri.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dcg.gaohongyu789.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vhv.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gtg.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://btp.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rdw.yonumen.top

Go:   // 手写 map[string][]T
来源：http://ssl.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ief.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uyw.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://ihb.pengpengdd.cyou

Py:   Counter(arr)
来源：http://iuj.tanke756.top

PHP:  array_count_values($arr);
来源：http://gpc.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bwp.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dyb.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://caq.c1oappe.top

Go:   // 手写 map[T]int
来源：http://hrz.haohaochexian.top

Ruby: arr.tally
来源：http://jax.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yeo.epnwcf.com

[D21] 判断是否包含某元素
来源：http://mzs.daria6918.cn

Py:   x in arr
来源：http://ssr.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://fmi.tarul.cn

JS:   arr.includes(x)
来源：http://mlr.kuanghao11.cn

TS:   arr.includes(x)
来源：http://tla.zdbjq.cn

Java: list.contains(x)
来源：http://siz.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://woz.ppjwa.cn

Ruby: arr.include?(x)
来源：http://twr.gzhubu.top

C#:   list.Contains(x)
来源：http://sau.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://cpy.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ktc.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://upf.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jlz.dianchejie.cn

TS:   [...arr];
来源：http://waa.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://bmx.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://gut.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://nfg.andypj.xyz

C#:   new List<int>(list);
来源：http://epy.cucudq.cn

[D23] reduce 累积计算
来源：http://tqy.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://twn.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ile.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jbh.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ion.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fzs.xuetiantiany.cn

Go:   // 手写循环
来源：http://nvl.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cmw.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hgl.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://zar.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gxe.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cry.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yki.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oug.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wvm.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iib.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rgp.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dri.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://iub.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vyl.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fih.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qry.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://csx.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nmp.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zqe.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sns.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xbb.smart0.xyz

[D26] 数组转字符串
来源：http://kjo.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://hct.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://yrl.yangfankeji.com

JS:   arr.join(", ")
来源：http://kdx.yfazqb.com

TS:   arr.join(", ")
来源：http://bja.guannengcc.top

Java: String.join(", ", list)
来源：http://qlb.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://jlb.cheryme.top

Ruby: arr.join(", ")
来源：http://hkn.xylfe.cn

C#:   string.Join(", ", list)
来源：http://iiv.xziqi.cn

================================================================================
来源：http://dnv.cqqwz.cn

E. 字符串处理
来源：http://omf.wangshuangyany.cn

================================================================================
来源：http://kdf.svipenyu.cn

[E01] 拼接字符串
来源：http://ulz.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kgz.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jup.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gqd.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jiu.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xsh.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ezs.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ygm.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmw.snrcjt.cn

[E02] 重复字符串
来源：http://wjd.yueranfly.top

Py:   "ab" * 3
来源：http://wsh.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://cge.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://uxa.cashguo.top

TS:   "ab".repeat(3)
来源：http://taz.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://rbt.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://gwi.hcnkem.com

Ruby: "ab" * 3
来源：http://ytj.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cqn.yueranfly.top

[E03] 截取子串
来源：http://zcj.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://deu.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tyc.pycfn.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mkq.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://jpx.ivvv.top

Java: s.substring(1, 4)
来源：http://cvg.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sti.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://usc.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://ipd.fktsv.cn

[E04] 查找子串位置
来源：http://wit.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://tvk.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://nww.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hev.hammf.cn

TS:   s.indexOf("x")
来源：http://tfi.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://syh.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://mkk.aizwys.cn

Ruby: s.index("x")
来源：http://gdu.jianghu66.top

C#:   s.IndexOf("x")
来源：http://fsv.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://yia.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://emn.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lvi.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxn.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qwv.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftp.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lwp.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jqg.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jpg.316326.xyz

[E06] 替换子串
来源：http://txx.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mxh.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://bmt.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eeq.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://gmm.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kab.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jbv.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ivy.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://ozc.redwolf501.top

[E07] 按分隔符拆分
来源：http://cmd.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oek.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vzj.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wft.jqgufenzy.top

TS:   s.split(",")
来源：http://tsb.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://hlg.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://omh.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://ufo.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://upj.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://gag.chenjidiqi.icu

Py:   ",".join(items)
来源：http://ghj.tianlin.xyz

PHP:  implode(",", $items);
来源：http://cav.aizwys.cn

JS:   items.join(",")
来源：http://ybo.hesvh.cn

TS:   items.join(",")
来源：http://nol.svipenyu.cn

Java: String.join(",", items)
来源：http://dns.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://muu.vqdsnc.cn

Ruby: items.join(",")
来源：http://thk.fktsv.cn

C#:   string.Join(",", items)
来源：http://hpe.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://msc.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://njm.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ffn.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://ecv.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://zcp.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://wgt.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wey.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ylz.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dno.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://cjj.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zzb.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ncu.sweek.top

JS:   "7".padStart(3, "0")
来源：http://mea.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://dzt.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://bee.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://zfe.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wgo.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zac.sjlbkw.cn

[E11] 反转字符串
来源：http://cos.jqgfzy.top

Py:   s[::-1]
来源：http://amf.yongpay.top

PHP:  strrev($s);
来源：http://nhd.zhiwuduotai.top


<!-- 参考信息 -->