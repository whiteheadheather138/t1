代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://icb.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://ytl.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://een.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://dnl.kuanghao11.cn

PHP:  sort($arr);
来源：http://amz.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://enz.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wow.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fvc.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rds.iojbl.cn

Ruby: arr.sort
来源：http://xva.shanyushiyangtech.top

C#:   list.Sort();
来源：http://ngq.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bcs.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lbx.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jfe.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yqn.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eeu.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qfo.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://juc.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lbo.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wep.pengpengdd.cyou

[D11] 反转数组
来源：http://gxv.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://awo.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://cai.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wne.316326.xyz

TS:   [...arr].reverse();
来源：http://egf.cashguo.top

Java: Collections.reverse(list);
来源：http://wxc.cheryme.top

Go:   slices.Reverse(arr)
来源：http://ahr.sufxvd.cn

Ruby: arr.reverse
来源：http://fes.chenjidiqi.icu

C#:   list.Reverse();
来源：http://doq.yj20258.top

[D12] 查找元素下标
来源：http://lko.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://vux.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iay.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eqo.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://spn.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rok.tarul.cn

Go:   slices.Index(arr, x)
来源：http://ufn.jlsjyb.cn

Ruby: arr.index(x)
来源：http://gvr.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://wsl.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://ioq.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hmw.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wyp.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://lho.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://qvp.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mzs.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jrf.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vmg.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hmz.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://wch.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oei.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xfh.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://iwo.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://lfr.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jte.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://kpm.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://rbh.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qzi.xziqi.cn

[D15] 去重
来源：http://yjp.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ulo.redwolf501.top

PHP:  array_unique($arr);
来源：http://qco.yongpay.top

JS:   [...new Set(arr)]
来源：http://lpd.smart0.xyz

TS:   [...new Set(arr)]
来源：http://wzp.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nin.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://qfa.gaohongyu789.top

Ruby: arr.uniq
来源：http://dqx.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://bme.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://iwn.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://olw.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yqo.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qnz.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgz.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zad.pycfn.com

Go:   // 手写循环累加
来源：http://you.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vca.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://qlg.nanxinkj.top

[D17] 最大值与最小值
来源：http://jpu.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://thx.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://neu.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xdc.chenzaomai.com

TS:   Math.max(...arr);
来源：http://fwe.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dez.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gbb.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://zei.316326.xyz

C#:   list.Max();  list.Min()
来源：http://pqt.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://nrc.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wem.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://yto.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cfh.fktsv.cn

TS:   nested.flat();
来源：http://opk.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vez.hesvh.cn

Go:   // 手写双层循环
来源：http://cca.ehwqpu.com

Ruby: nested.flatten
来源：http://odn.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nww.ivvv.top

[D19] 按字段分组
来源：http://lvo.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vzq.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kfg.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kkg.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dug.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gvk.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://woe.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yco.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fxq.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://gmj.tarul.cn

Py:   Counter(arr)
来源：http://ezg.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://jmh.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lcc.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rbe.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aun.mhx1999.top

Go:   // 手写 map[T]int
来源：http://ndd.xziqi.cn

Ruby: arr.tally
来源：http://yga.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iai.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://lkj.bbcook.cn

Py:   x in arr
来源：http://ikv.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://wbp.jyoumei.cn

JS:   arr.includes(x)
来源：http://plg.yueranfly.top

TS:   arr.includes(x)
来源：http://ssd.shzxlz.cn

Java: list.contains(x)
来源：http://cse.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://fgc.sysykeji.top

Ruby: arr.include?(x)
来源：http://ecy.wangdashe.top

C#:   list.Contains(x)
来源：http://asy.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://cbz.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gyc.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uxt.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://efo.fktsv.cn

TS:   [...arr];
来源：http://ixs.hnqzz.top

Java: new ArrayList<>(list);
来源：http://tcn.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://saz.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://oxy.gzhubu.top

C#:   new List<int>(list);
来源：http://oxv.zdbjq.cn

[D23] reduce 累积计算
来源：http://wyz.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zjw.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mgh.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wxq.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfn.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nib.gogol.net.cn

Go:   // 手写循环
来源：http://web.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gai.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dtn.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://qxo.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://odl.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mmk.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blc.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nzm.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ujn.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hsg.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uvg.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://szb.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://umn.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zbk.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sqf.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tai.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://avy.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gff.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uuk.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://inn.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pia.hammf.cn

[D26] 数组转字符串
来源：http://jwg.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://pzp.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://lzf.nanxinkj.top

JS:   arr.join(", ")
来源：http://dzv.jinqigufen.top

TS:   arr.join(", ")
来源：http://znv.jqgfzy.top

Java: String.join(", ", list)
来源：http://rmj.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://lkf.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://clv.vehdjk.com

C#:   string.Join(", ", list)
来源：http://jyd.hesvh.cn

================================================================================
来源：http://gdr.guowangkeji.top

E. 字符串处理
来源：http://zyw.kuanghao11.cn

================================================================================
来源：http://tsn.jlsjyb.cn

[E01] 拼接字符串
来源：http://dai.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hvo.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rkl.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgc.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jug.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qmu.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vdi.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zfm.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pba.feifeiyinyue.top

[E02] 重复字符串
来源：http://jas.mhx1999.top

Py:   "ab" * 3
来源：http://ovf.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://ntg.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://mvr.52xcode.cn

TS:   "ab".repeat(3)
来源：http://cmx.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://cau.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://fld.0kj1m.cn

Ruby: "ab" * 3
来源：http://puz.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://daz.gaohongyu789.top

[E03] 截取子串
来源：http://shf.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vdg.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dpf.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://phg.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://xcy.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://den.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://byc.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://ssu.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://ubz.redwolf501.top

[E04] 查找子串位置
来源：http://qwl.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://ims.andypj.xyz

PHP:  strpos($s, "x");
来源：http://jje.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vqf.dashuyun.cn

TS:   s.indexOf("x")
来源：http://gex.redwolf501.top

Java: s.indexOf("x")
来源：http://vcz.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://efu.dianchejie.cn

Ruby: s.index("x")
来源：http://eac.52xcode.cn

C#:   s.IndexOf("x")
来源：http://oco.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kgu.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://any.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iej.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eih.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://ibj.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxu.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zhe.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xvf.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://klw.jyoumei.cn

[E06] 替换子串
来源：http://lms.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qgz.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://npi.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tny.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://ogr.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hoj.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://far.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://txi.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://owo.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://nlt.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ffn.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ftv.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gnf.zhoulong.xyz

TS:   s.split(",")
来源：http://pdb.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://wtp.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vgu.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://dqe.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xdi.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://ojb.wangshuangyany.cn

Py:   ",".join(items)
来源：http://bzf.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://rxl.yuxming.cn

JS:   items.join(",")
来源：http://ueg.jlsjyb.cn

TS:   items.join(",")
来源：http://dsw.aibaodan.cn

Java: String.join(",", items)
来源：http://qoy.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://ewr.gzhubu.top

Ruby: items.join(",")
来源：http://lxr.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://tbq.shzxlz.cn

[E09] 去除所有空白字符
来源：http://ykv.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ysg.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ixt.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://tjc.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://thj.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://pao.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xcv.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ltf.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dun.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://diu.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rpw.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nii.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://sli.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://rrc.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://sku.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://glr.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zzr.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sqh.fengsongda.top

[E11] 反转字符串
来源：http://xqr.jinqigufen.top

Py:   s[::-1]
来源：http://fgm.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://skv.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://tba.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://twz.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mib.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://efk.316326.xyz

Ruby: s.reverse
来源：http://hot.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ohb.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://tlg.jinqigufen.top

Py:   s.count("a")
来源：http://gtl.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://umn.andypj.xyz

JS:   s.split("a").length - 1
来源：http://ghd.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://bxj.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rtm.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://ghy.tarul.cn

Ruby: s.count("a")
来源：http://bgi.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://bxx.jinqigfzy.top

[E13] 逐字符遍历
来源：http://xwz.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://nez.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hol.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oiq.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://nja.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yhv.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xbo.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://alx.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oxu.ydzc1.top

[E14] URL 编码与 Base64
来源：http://res.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwm.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rpu.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://urc.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rnb.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jzi.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gam.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pfa.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rnp.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://tci.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://niz.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jaf.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://egh.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ief.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dac.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qyx.316326.xyz


<!-- 参考信息 -->