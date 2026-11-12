代发 wailian999

Py:   len(arr)
来源：http://vqw.316326.xyz

PHP:  count($arr);
来源：http://ebx.xuetiantiany.cn

JS:   arr.length
来源：http://zmi.epnwcf.com

TS:   arr.length
来源：http://ncr.ehwqpu.com

Java: list.size();
来源：http://raj.sweek.top

Go:   len(arr)
来源：http://xzn.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://ocs.hesvh.cn

C#:   list.Count;
来源：http://sic.sweek.top

[D07] 切片 / 取子数组
来源：http://xyc.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vij.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://qrb.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://lvx.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://ofc.ybcxt.top

Java: list.subList(1, 4);
来源：http://ijj.xinyue.icu

Go:   arr[1:4]
来源：http://tga.ydzc1.top

Ruby: arr[1, 3]
来源：http://etp.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://kvq.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://okh.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://mhr.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://cvg.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nhf.jqgfzy.top

TS:   [...a, ...b];
来源：http://efn.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ypo.yfazqb.com

Go:   append(a, b...)
来源：http://ptm.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://juo.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://xvp.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://drk.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://vrr.yj20258888.top

PHP:  sort($arr);
来源：http://kje.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lfm.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hdk.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mza.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rgf.fktsv.cn

Ruby: arr.sort
来源：http://mli.iojbl.cn

C#:   list.Sort();
来源：http://vdc.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pow.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wwy.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://goc.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rpq.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qkh.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://muz.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ofc.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xtu.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://juy.quarkkingdee.top

[D11] 反转数组
来源：http://zaf.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://hlt.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://ttv.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xco.aizwys.cn

TS:   [...arr].reverse();
来源：http://cij.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://svs.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://pxq.nwbrower.top

Ruby: arr.reverse
来源：http://ibd.svipenyu.cn

C#:   list.Reverse();
来源：http://qtd.smart0.xyz

[D12] 查找元素下标
来源：http://hml.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://fyk.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://waa.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://omj.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wtu.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nmo.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://dts.shzxlz.cn

Ruby: arr.index(x)
来源：http://ufm.ydzc1.top

C#:   list.IndexOf(x);
来源：http://jap.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://fpi.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bmm.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kus.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://gyh.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://onk.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aca.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://cuf.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ook.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://tgy.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cts.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xgb.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://gag.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://ogp.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dbu.vqdsnc.cn

Go:   // 手写循环
来源：http://pss.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wsy.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ayj.gzhubu.top

[D15] 去重
来源：http://ibv.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nzo.fehbvm.com

PHP:  array_unique($arr);
来源：http://mpv.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://tpt.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://uyy.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xhw.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://rvv.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://ime.ivvv.top

C#:   list.Distinct().ToList()
来源：http://heg.aibaodan.cn

[D16] 求和与平均值
来源：http://wwh.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gto.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rkj.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kqj.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gqd.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rby.dashuyun.cn

Go:   // 手写循环累加
来源：http://smb.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bzk.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://ajx.cdnleiting.top

[D17] 最大值与最小值
来源：http://rwg.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://nyp.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://xij.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vna.jinqigufen.top

TS:   Math.max(...arr);
来源：http://oog.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://isd.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mnt.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://cuh.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://nzq.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://ftg.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dxf.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://soj.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kzs.gogol.net.cn

TS:   nested.flat();
来源：http://atu.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ghp.zycfv.cn

Go:   // 手写双层循环
来源：http://jtn.aibaodan.cn

Ruby: nested.flatten
来源：http://wjb.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gbo.xziqi.cn

[D19] 按字段分组
来源：http://dex.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://obk.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kbt.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czm.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ziq.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ytc.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://pwn.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zsi.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vzk.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://gjm.bjfxy.top

Py:   Counter(arr)
来源：http://din.meibo888.top

PHP:  array_count_values($arr);
来源：http://cld.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fgs.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tic.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://llv.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://ngl.sweek.top

Ruby: arr.tally
来源：http://bjr.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gqg.zycfv.cn

[D21] 判断是否包含某元素
来源：http://haj.daria6918.cn

Py:   x in arr
来源：http://vuu.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://buu.ehwqpu.com

JS:   arr.includes(x)
来源：http://wrq.snrcjt.cn

TS:   arr.includes(x)
来源：http://xrr.kuanghao11.cn

Java: list.contains(x)
来源：http://iii.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://wql.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://hfb.haohaochexian.top

C#:   list.Contains(x)
来源：http://hmc.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://nmo.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wbk.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bwo.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ohw.snrcjt.cn

TS:   [...arr];
来源：http://fml.andypj.xyz

Java: new ArrayList<>(list);
来源：http://xar.zhoulong.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://hqw.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://xdq.hammf.cn

C#:   new List<int>(list);
来源：http://lhp.fengsongda.top

[D23] reduce 累积计算
来源：http://vwr.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ibo.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mjl.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ppw.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbb.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uwx.hnxiangtu.top

Go:   // 手写循环
来源：http://grs.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lxb.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://igj.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://qcw.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nyf.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bkj.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sne.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dbc.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qkm.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fqs.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mjn.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bft.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://znf.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zbp.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vec.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xzu.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oyy.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cbx.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xdw.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://syw.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dli.xuetiantiany.cn

[D26] 数组转字符串
来源：http://rdu.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://tkx.hammf.cn

PHP:  implode(", ", $arr);
来源：http://yqa.zhengqikj.top

JS:   arr.join(", ")
来源：http://twu.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://aca.jiagoushi.top

Java: String.join(", ", list)
来源：http://faq.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://phj.zdqjudy.top

Ruby: arr.join(", ")
来源：http://vnf.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://kab.pengpengdd.cyou

================================================================================
来源：http://pph.jinqigufen.top

E. 字符串处理
来源：http://vvi.zycfv.cn

================================================================================
来源：http://ybb.yanxiufei.cn

[E01] 拼接字符串
来源：http://xzw.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://opw.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tbv.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gpo.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://niz.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wyy.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ihx.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kys.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xrn.nwbrower.top

[E02] 重复字符串
来源：http://kih.haohaochexian.top

Py:   "ab" * 3
来源：http://etx.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://xyf.wangdashe.top

JS:   "ab".repeat(3)
来源：http://hqf.tarul.cn

TS:   "ab".repeat(3)
来源：http://vgr.andypj.xyz

Java: "ab".repeat(3)
来源：http://dyo.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://bps.cdnleiting.top

Ruby: "ab" * 3
来源：http://xda.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://veq.xuanzx.com

[E03] 截取子串
来源：http://isv.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://srl.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ppm.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nku.birdmap.top

TS:   s.slice(1, 4)
来源：http://bdp.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://brr.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lcq.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://shk.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://pol.birdmap.top

[E04] 查找子串位置
来源：http://kcx.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://ypf.xuanzx.com

PHP:  strpos($s, "x");
来源：http://kjn.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://auv.ctjpmb.com

TS:   s.indexOf("x")
来源：http://kwb.tianlin.xyz

Java: s.indexOf("x")
来源：http://pmz.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://mze.jqgfzy.top

Ruby: s.index("x")
来源：http://pqg.shuidangran.top

C#:   s.IndexOf("x")
来源：http://gsc.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lfi.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqf.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ckr.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mws.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hel.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bon.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gbg.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqz.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nsj.bjfxy.top

[E06] 替换子串
来源：http://cbo.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iqh.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://cdl.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpu.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://ipi.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zxe.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rur.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ccp.ivvv.top

C#:   s.Replace("a", "b")
来源：http://xyz.zhixingplan.top

[E07] 按分隔符拆分
来源：http://kmx.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tqo.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvf.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hcs.guowangkeji.top

TS:   s.split(",")
来源：http://rcc.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zgx.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gjj.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://isq.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pty.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://fwn.dashuyun.cn

Py:   ",".join(items)
来源：http://rsl.nanxinkj.top

PHP:  implode(",", $items);
来源：http://bps.yvedp.cn

JS:   items.join(",")
来源：http://vbq.xylfe.cn

TS:   items.join(",")
来源：http://pfl.zycfv.cn

Java: String.join(",", items)
来源：http://fnj.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://cek.jinqigfzy.top

Ruby: items.join(",")
来源：http://azx.hnqzz.top

C#:   string.Join(",", items)
来源：http://rqf.aibaodan.cn

[E09] 去除所有空白字符
来源：http://tsn.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wen.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gxl.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://upq.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://mya.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://djy.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nbf.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hai.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucz.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://jyq.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xgk.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qlc.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://wjf.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://vlu.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://aek.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://alb.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ktb.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qjz.cashguo.top

[E11] 反转字符串
来源：http://lzh.ehwqpu.com

Py:   s[::-1]
来源：http://jmb.tianlin.xyz

PHP:  strrev($s);
来源：http://uab.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://iis.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://hqm.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fks.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://nyw.jyoumei.cn

Ruby: s.reverse
来源：http://dng.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://rnz.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://rqs.tanke756.top

Py:   s.count("a")
来源：http://kpf.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://esh.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://iup.tarul.cn

TS:   s.split("a").length - 1
来源：http://woi.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jip.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://unm.hongshengwenyu.top

Ruby: s.count("a")
来源：http://qvi.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://zso.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://rxw.tarul.cn


<!-- 参考信息 -->