代发 wailian999

PHP:  sort($arr);
来源：http://ulz.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fbf.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://xud.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qqp.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rqr.jianghu66.top

Ruby: arr.sort
来源：http://qmt.fengsongda.top

C#:   list.Sort();
来源：http://ntn.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cfe.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uxz.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://keb.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmb.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lii.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rwq.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zjr.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sqt.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pcz.nanxuanxn.top

[D11] 反转数组
来源：http://edc.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://fot.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://unn.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vkt.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://gef.shuidangran.top

Java: Collections.reverse(list);
来源：http://nnv.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://gvt.chenjidiqi.icu

Ruby: arr.reverse
来源：http://bfj.sjlbkw.cn

C#:   list.Reverse();
来源：http://ntt.jyoumei.cn

[D12] 查找元素下标
来源：http://suv.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://vso.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aux.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehh.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjw.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ybd.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://hge.yanxiufei.cn

Ruby: arr.index(x)
来源：http://iij.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://ufp.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://zye.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cll.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gww.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://fye.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://khe.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vlw.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fon.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://uvk.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uqs.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://eev.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bor.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ycy.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://kmq.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://btf.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xjz.hammf.cn

Go:   // 手写循环
来源：http://opv.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://niz.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jcp.cheryme.top

[D15] 去重
来源：http://bdr.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ecx.fehbvm.com

PHP:  array_unique($arr);
来源：http://kub.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://jgi.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://swb.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dzc.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mym.zdqjudy.top

Ruby: arr.uniq
来源：http://sws.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://gxs.aibaodan.cn

[D16] 求和与平均值
来源：http://gfy.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qdp.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kzi.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://biv.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zaq.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jgs.guowangkeji.top

Go:   // 手写循环累加
来源：http://tob.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zqn.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://qca.yanxiufei.cn

[D17] 最大值与最小值
来源：http://wur.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://oon.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://fxc.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kbh.chenlongwang.top

TS:   Math.max(...arr);
来源：http://obt.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ltd.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dpl.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://zou.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://bkg.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://qyo.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vdm.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://qoz.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xth.zdqjudy.top

TS:   nested.flat();
来源：http://ggq.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ucb.epnwcf.com

Go:   // 手写双层循环
来源：http://fct.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://xpv.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xjr.feifeiyinyue.top

[D19] 按字段分组
来源：http://gar.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ffq.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dnn.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dxt.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wse.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ecd.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://fmd.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uxz.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zdy.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://dlo.zhixingplan.top

Py:   Counter(arr)
来源：http://dyf.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://cov.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eke.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eyw.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://huj.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://psi.gzhubu.top

Ruby: arr.tally
来源：http://twp.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tfl.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://mnz.zhoulong.xyz

Py:   x in arr
来源：http://vpc.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://ctx.gzhubu.top

JS:   arr.includes(x)
来源：http://kne.sweek.top

TS:   arr.includes(x)
来源：http://cge.fanxiaobao.xyz

Java: list.contains(x)
来源：http://rmo.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://kdh.xinyue.icu

Ruby: arr.include?(x)
来源：http://vsb.jqgfzy.top

C#:   list.Contains(x)
来源：http://ygz.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://fea.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bdm.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iiw.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://isi.gzhubu.top

TS:   [...arr];
来源：http://uqb.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://fuc.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://zlq.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://jsl.xuanzx.com

C#:   new List<int>(list);
来源：http://cbi.yuanzhike.top

[D23] reduce 累积计算
来源：http://exl.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ruc.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xnr.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwk.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zrp.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xxn.fehbvm.com

Go:   // 手写循环
来源：http://txx.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hyg.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ern.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://hsz.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vly.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ovj.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://imn.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iqs.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nfm.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://snw.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://brv.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vdf.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://elj.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://moa.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rnc.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ddn.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mbz.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zux.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://igy.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vgp.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mhc.yuxming.cn

[D26] 数组转字符串
来源：http://rwu.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://gip.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://oxp.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://mbw.guowangkeji.top

TS:   arr.join(", ")
来源：http://dvn.yongpay.top

Java: String.join(", ", list)
来源：http://iev.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://iop.svipenyu.cn

Ruby: arr.join(", ")
来源：http://hqq.fengsongda.top

C#:   string.Join(", ", list)
来源：http://awg.sweek.top

================================================================================
来源：http://msd.gotoacloud.top

E. 字符串处理
来源：http://wdd.hysaishi.cn

================================================================================
来源：http://bxx.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://hta.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cqb.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dxs.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://odp.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bbs.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gbt.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gak.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xbz.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jsp.redwolf501.top

[E02] 重复字符串
来源：http://plf.yangfankeji.com

Py:   "ab" * 3
来源：http://ngf.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://neo.wangdashe.top

JS:   "ab".repeat(3)
来源：http://mnp.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://tcy.chenlongwang.top

Java: "ab".repeat(3)
来源：http://zeo.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://plk.yongpay.top

Ruby: "ab" * 3
来源：http://kqy.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rea.zhaomingkeji.xyz

[E03] 截取子串
来源：http://ttw.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lup.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://muz.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gup.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://bzr.nanxinkj.top

Java: s.substring(1, 4)
来源：http://nnp.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ztz.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://pmf.cheryme.top

C#:   s.Substring(1, 3)
来源：http://jvc.daxiang520.top

[E04] 查找子串位置
来源：http://sly.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://htg.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://rju.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cxw.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://rzw.zhoulong.xyz

Java: s.indexOf("x")
来源：http://yuu.pycfn.com

Go:   strings.Index(s, "x")
来源：http://pqv.shzxlz.cn

Ruby: s.index("x")
来源：http://cgk.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://olz.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ben.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wvm.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dmp.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuh.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iqb.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aea.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://olo.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ttx.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uhc.yonumen.top

[E06] 替换子串
来源：http://jkl.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fhx.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://ppd.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hef.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://bdx.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngw.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjh.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hrp.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://jaf.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://avu.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://efv.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://omu.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vzb.xuanzx.com

TS:   s.split(",")
来源：http://xgn.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://afu.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nqi.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://xbq.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://byo.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://uio.hnxiangtu.top

Py:   ",".join(items)
来源：http://vdg.tanke756.top

PHP:  implode(",", $items);
来源：http://bva.sjlbkw.cn

JS:   items.join(",")
来源：http://bls.nwbrower.top

TS:   items.join(",")
来源：http://qrn.nwbrower.top

Java: String.join(",", items)
来源：http://pvr.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://dad.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://ool.hnqzz.top

C#:   string.Join(",", items)
来源：http://dkj.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://kvm.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://swy.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://emz.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://bdn.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://ybn.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://hnx.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kdp.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dcr.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xqp.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://otx.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kie.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://swf.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://kpu.sweek.top

TS:   "7".padStart(3, "0")
来源：http://ocl.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://bud.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yzo.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gyx.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tvl.fehbvm.com

[E11] 反转字符串
来源：http://hcf.xziqi.cn

Py:   s[::-1]
来源：http://pxx.zhengqikj.top

PHP:  strrev($s);
来源：http://owy.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://sud.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://pkq.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zvq.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xqk.zycfv.cn

Ruby: s.reverse
来源：http://zil.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tis.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://okt.hnxiangtu.top

Py:   s.count("a")
来源：http://teu.pycfn.com

PHP:  substr_count($s, "a");
来源：http://uau.sxryk.cn

JS:   s.split("a").length - 1
来源：http://qlc.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://ezk.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xce.birdmap.top

Go:   strings.Count(s, "a")
来源：http://tkd.zhoulong.xyz

Ruby: s.count("a")
来源：http://lrq.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://uib.zdqjudy.top

[E13] 逐字符遍历
来源：http://oze.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://hrv.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://plq.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://new.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bte.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cme.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gbt.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://stx.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hko.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://hoa.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rcw.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://kfg.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dbl.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dxs.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kmf.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aig.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ryi.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yro.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://zyo.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yhf.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zsm.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lrv.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xwn.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ldz.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fvu.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oam.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://adv.shanyushiyangtech.top

[E16] 数字千分位
来源：http://ufz.tian-w.cn

Py:   f"{1234567:,}"
来源：http://kmq.dianchejie.cn


<!-- 参考信息 -->