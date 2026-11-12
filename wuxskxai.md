代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://idv.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxv.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://krb.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntx.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oze.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jkn.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hjv.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hbx.zhijiandao.cn

[D11] 反转数组
来源：http://cvm.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://hik.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://sjz.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dji.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://chh.gogol.net.cn

Java: Collections.reverse(list);
来源：http://bki.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://djq.svipenyu.cn

Ruby: arr.reverse
来源：http://gvx.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://ogv.hongshengwenyu.top

[D12] 查找元素下标
来源：http://kbh.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://udl.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tjv.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://skd.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihl.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vtx.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://pdi.ctjpmb.com

Ruby: arr.index(x)
来源：http://xmy.bjfxy.top

C#:   list.IndexOf(x);
来源：http://eps.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://gvc.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lrn.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mbh.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://hui.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://hvy.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cqt.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wno.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ddm.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wxc.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://yry.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fqu.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zvw.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://kqh.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://zua.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ldy.tanke756.top

Go:   // 手写循环
来源：http://skf.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uye.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://lfs.jinqigufen.top

[D15] 去重
来源：http://ykg.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tjc.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://zzu.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://xra.cucudq.cn

TS:   [...new Set(arr)]
来源：http://xqe.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsb.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yxa.cashguo.top

Ruby: arr.uniq
来源：http://xwv.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://rax.ivvv.top

[D16] 求和与平均值
来源：http://beu.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bic.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kbw.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dhq.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://otf.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://znt.vehdjk.com

Go:   // 手写循环累加
来源：http://vlg.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qzj.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://xai.xuanzx.com

[D17] 最大值与最小值
来源：http://rgq.cheryme.top

Py:   max(arr);  min(arr)
来源：http://szf.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://qlp.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wcv.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://jum.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mvi.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://igr.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://gzm.cheryme.top

C#:   list.Max();  list.Min()
来源：http://fgj.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://cce.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uwf.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://sxv.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fjb.zhixingplan.top

TS:   nested.flat();
来源：http://daf.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://emg.tanke756.top

Go:   // 手写双层循环
来源：http://pfs.yuxming.cn

Ruby: nested.flatten
来源：http://ufi.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://snx.zdbjq.cn

[D19] 按字段分组
来源：http://gox.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ioy.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xle.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://isa.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ksm.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dmt.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://vtr.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://gbo.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qho.316326.xyz

[D20] 统计每个元素出现次数
来源：http://dkf.fzhhl.top

Py:   Counter(arr)
来源：http://tgb.yongpay.top

PHP:  array_count_values($arr);
来源：http://nwh.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwr.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pjp.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jsb.yj202588.top

Go:   // 手写 map[T]int
来源：http://kba.cucudq.cn

Ruby: arr.tally
来源：http://cwc.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ywq.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://pxg.yfazqb.com

Py:   x in arr
来源：http://lsa.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://igf.mhx1999.top

JS:   arr.includes(x)
来源：http://gpb.bjfxy.top

TS:   arr.includes(x)
来源：http://qzt.redwolf501.top

Java: list.contains(x)
来源：http://pvh.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://xil.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://ppk.shzxlz.cn

C#:   list.Contains(x)
来源：http://ubi.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://apa.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gmg.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gfe.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mob.wangdashe.top

TS:   [...arr];
来源：http://iqi.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://gsh.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://wrx.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://tnk.kuanghao11.cn

C#:   new List<int>(list);
来源：http://pea.hfpthk.cn

[D23] reduce 累积计算
来源：http://rfv.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hwk.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mbg.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wmx.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xpc.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lzx.haohaochexian.top

Go:   // 手写循环
来源：http://bos.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pmm.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kbv.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://hra.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zak.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ale.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vbm.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fzi.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ljt.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://urg.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://spq.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fzw.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://lol.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lds.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nwm.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tvs.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://arn.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vjh.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nhf.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ofz.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bny.cashguo.top

[D26] 数组转字符串
来源：http://iya.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://ogi.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://bod.9152youxi.cn

JS:   arr.join(", ")
来源：http://sht.fehbvm.com

TS:   arr.join(", ")
来源：http://lej.yongpay.top

Java: String.join(", ", list)
来源：http://gov.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://ncs.vehdjk.com

Ruby: arr.join(", ")
来源：http://tot.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://fwa.shanyushiyangtech.top

================================================================================
来源：http://chg.316326.xyz

E. 字符串处理
来源：http://hvm.0kj1m.cn

================================================================================
来源：http://tor.vehdjk.com

[E01] 拼接字符串
来源：http://hir.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cvd.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ogk.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ydr.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iek.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pqi.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cbt.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://osx.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ytn.vehdjk.com

[E02] 重复字符串
来源：http://fwq.hammf.cn

Py:   "ab" * 3
来源：http://jab.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://wbp.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://rsc.yuxming.cn

TS:   "ab".repeat(3)
来源：http://wih.yj202588.top

Java: "ab".repeat(3)
来源：http://lkq.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://ojz.ybcxt.top

Ruby: "ab" * 3
来源：http://pyh.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wvi.yfazqb.com

[E03] 截取子串
来源：http://jqg.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cgg.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ulw.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jmt.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://cvj.hywenlv.cn

Java: s.substring(1, 4)
来源：http://tnd.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://roe.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://vev.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://pla.nanxinkj.top

[E04] 查找子串位置
来源：http://bqp.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://vnb.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://nwa.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oba.wangdashe.top

TS:   s.indexOf("x")
来源：http://hsg.redwolf501.top

Java: s.indexOf("x")
来源：http://smz.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://xlu.gogol.net.cn

Ruby: s.index("x")
来源：http://pbs.andypj.xyz

C#:   s.IndexOf("x")
来源：http://pbz.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jdd.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ipj.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mgx.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gzr.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vhg.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://opb.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yig.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://abf.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uoj.shanyushiyangkeji.top

[E06] 替换子串
来源：http://lmg.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fmf.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://lca.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ciw.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://gqz.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://plh.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uwg.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://msv.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://avo.gogol.net.cn

[E07] 按分隔符拆分
来源：http://tvu.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kup.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rwj.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://bzn.bbcook.cn

TS:   s.split(",")
来源：http://ned.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://kpb.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qty.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://jiu.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://avy.daxiang520.top

[E08] 数组按分隔符合并
来源：http://gxo.hysaishi.cn

Py:   ",".join(items)
来源：http://dwa.ybcxt.top

PHP:  implode(",", $items);
来源：http://rwt.sweek.top

JS:   items.join(",")
来源：http://vrb.tarul.cn

TS:   items.join(",")
来源：http://tic.yangfankeji.com

Java: String.join(",", items)
来源：http://ltl.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://okp.hammf.cn

Ruby: items.join(",")
来源：http://zgy.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://ahe.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://fqf.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mom.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uej.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://ddh.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://dbs.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://dnh.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ejl.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://rdk.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hpv.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://rng.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xon.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gym.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://gdi.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://mcz.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://wjd.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lkg.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://voh.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fra.yueranfly.top

[E11] 反转字符串
来源：http://pxh.ybcxt.top

Py:   s[::-1]
来源：http://pfl.sufxvd.cn

PHP:  strrev($s);
来源：http://gas.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://pzu.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://vlp.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sch.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://aea.aizwys.cn

Ruby: s.reverse
来源：http://zvy.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://sgx.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://xos.jinqigfzy.top

Py:   s.count("a")
来源：http://pnt.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://mmf.xziqi.cn

JS:   s.split("a").length - 1
来源：http://zys.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://mfn.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ilr.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://poo.daxiang520.top

Ruby: s.count("a")
来源：http://rht.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://yod.yueranfly.top

[E13] 逐字符遍历
来源：http://kfb.tarul.cn

Py:   for ch in s: print(ch)
来源：http://yve.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvr.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hsr.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rfn.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yts.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zdj.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lan.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hah.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://shb.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hjj.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hpf.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ble.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://loq.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igo.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jqp.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gac.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mlz.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://arg.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dlk.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nkc.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://esz.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gou.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xon.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ptg.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gwa.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpa.jyoumei.cn

[E16] 数字千分位
来源：http://ynu.yongpay.top

Py:   f"{1234567:,}"
来源：http://pug.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://sif.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hxe.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ubx.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://reo.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ddi.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pqj.cheryme.top

C#:   1234567.ToString("N0")
来源：http://gsa.jyoumei.cn

[E17] 首字母大写
来源：http://fwi.sufxvd.cn


<!-- 参考信息 -->