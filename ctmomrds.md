代发 wailian999

Ruby: arr.index(x)
来源：http://uqg.yuxming.cn

C#:   list.IndexOf(x);
来源：http://rmi.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://dla.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ufs.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sdb.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://wun.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://upr.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fzq.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fjz.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://aoo.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qnt.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://pwz.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fxk.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qfj.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://tqx.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://oji.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cwq.xinyue.icu

Go:   // 手写循环
来源：http://atp.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://roj.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://qky.hcnkem.com

[D15] 去重
来源：http://oyc.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vbz.cdnleiting.top

PHP:  array_unique($arr);
来源：http://slk.fehbvm.com

JS:   [...new Set(arr)]
来源：http://oau.pycfn.com

TS:   [...new Set(arr)]
来源：http://igm.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yet.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://zdi.nwbrower.top

Ruby: arr.uniq
来源：http://dde.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://uyk.cucudq.cn

[D16] 求和与平均值
来源：http://ohn.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uta.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yxe.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ikc.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aps.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jyn.xylfe.cn

Go:   // 手写循环累加
来源：http://dmc.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cjo.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://smq.fktsv.cn

[D17] 最大值与最小值
来源：http://qow.cashguo.top

Py:   max(arr);  min(arr)
来源：http://mln.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://hgy.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://get.bjfxy.top

TS:   Math.max(...arr);
来源：http://sdx.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://asj.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jrj.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://xyp.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://aoq.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://hsj.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://npd.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://cvu.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jyr.jqgfzy.top

TS:   nested.flat();
来源：http://esm.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rhu.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://krq.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://kqk.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kmn.sweek.top

[D19] 按字段分组
来源：http://kau.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ogh.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tid.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ixa.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fbc.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hkl.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://lml.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://cam.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kdp.yj20258.top

[D20] 统计每个元素出现次数
来源：http://age.yuxming.cn

Py:   Counter(arr)
来源：http://rai.havefunace.top

PHP:  array_count_values($arr);
来源：http://bfm.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://key.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dpu.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cqx.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://pvv.dianchejie.cn

Ruby: arr.tally
来源：http://xaz.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vaw.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://jwe.cucudq.cn

Py:   x in arr
来源：http://xgj.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://qqg.sjlbkw.cn

JS:   arr.includes(x)
来源：http://glm.zhijiandao.cn

TS:   arr.includes(x)
来源：http://ekm.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://qby.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://pyi.snrcjt.cn

Ruby: arr.include?(x)
来源：http://bda.cqqwz.cn

C#:   list.Contains(x)
来源：http://hmc.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://igw.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://red.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vba.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://njx.ehwqpu.com

TS:   [...arr];
来源：http://xen.yueranfly.top

Java: new ArrayList<>(list);
来源：http://uzx.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cqv.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://gri.yongpay.top

C#:   new List<int>(list);
来源：http://szm.yangfankeji.com

[D23] reduce 累积计算
来源：http://ifn.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sed.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kav.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://weo.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://npp.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ffr.yfazqb.com

Go:   // 手写循环
来源：http://von.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://emn.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zev.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://rbj.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vdr.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rsv.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oqh.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yhl.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jfk.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://umh.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bmb.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dnp.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://kgr.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yoh.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xxm.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ygg.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dog.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qvw.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sxp.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zit.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tfi.haohaochexian.top

[D26] 数组转字符串
来源：http://zxe.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://klj.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://ykc.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://kqa.kuanghao11.cn

TS:   arr.join(", ")
来源：http://shk.ehwqpu.com

Java: String.join(", ", list)
来源：http://yif.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://fcf.zycfv.cn

Ruby: arr.join(", ")
来源：http://vgz.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://gop.cdnleiting.top

================================================================================
来源：http://gjd.yvedp.cn

E. 字符串处理
来源：http://syh.fktsv.cn

================================================================================
来源：http://sxy.gaohongyu789.top

[E01] 拼接字符串
来源：http://ugl.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ciy.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zre.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrm.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lte.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fky.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xbj.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hxw.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uid.zhixingplan.top

[E02] 重复字符串
来源：http://bng.yvedp.cn

Py:   "ab" * 3
来源：http://pti.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://ypy.fengsongda.top

JS:   "ab".repeat(3)
来源：http://qgn.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://our.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://vfn.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://ast.fzhhl.top

Ruby: "ab" * 3
来源：http://kjy.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://enu.hywenlv.cn

[E03] 截取子串
来源：http://ema.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nbw.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bqn.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zyh.sxryk.cn

TS:   s.slice(1, 4)
来源：http://dow.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://zsa.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hkt.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kjk.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://fui.meibo888.top

[E04] 查找子串位置
来源：http://orh.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://fmr.sjlbkw.cn

PHP:  strpos($s, "x");
来源：http://qci.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mon.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://lsy.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://gnm.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://njq.ybcxt.top

Ruby: s.index("x")
来源：http://rxh.bjfxy.top

C#:   s.IndexOf("x")
来源：http://cws.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zma.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xzt.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pln.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uwg.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://boq.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ebn.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bmb.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pzy.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rsy.zhaomingkeji.xyz

[E06] 替换子串
来源：http://cjb.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lfy.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://kwm.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nuj.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://agh.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oyw.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kzo.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vqv.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://vkv.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://wfu.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tke.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://txo.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bmr.yueranfly.top

TS:   s.split(",")
来源：http://tlr.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://spo.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nqb.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://yro.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lpu.jianghu66.top

[E08] 数组按分隔符合并
来源：http://qux.cqqwz.cn

Py:   ",".join(items)
来源：http://sev.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://hmk.52xcode.cn

JS:   items.join(",")
来源：http://vmb.zycfv.cn

TS:   items.join(",")
来源：http://hxb.kuanghao11.cn

Java: String.join(",", items)
来源：http://ekq.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://fmg.zycfv.cn

Ruby: items.join(",")
来源：http://kfe.snrcjt.cn

C#:   string.Join(",", items)
来源：http://fhz.epnwcf.com

[E09] 去除所有空白字符
来源：http://jcb.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gid.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ssc.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://tew.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://jlz.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://ykf.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://gsz.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://pzm.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xop.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://ylf.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://exg.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://otn.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://nvo.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://sis.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://lyu.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lgq.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pcg.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tgy.hnqzz.top

[E11] 反转字符串
来源：http://tzr.feifeiyinyue.top

Py:   s[::-1]
来源：http://dga.sweek.top

PHP:  strrev($s);
来源：http://uxo.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://ipj.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://zuz.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wnm.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hxb.shanyushiyangtech.top

Ruby: s.reverse
来源：http://kuq.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://hmk.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://npe.pycfn.com

Py:   s.count("a")
来源：http://uqw.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://spe.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://xoo.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://gij.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zwp.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://zxd.guowangkeji.top

Ruby: s.count("a")
来源：http://wvz.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://gwn.meibo888.top

[E13] 逐字符遍历
来源：http://pes.havefunace.top

Py:   for ch in s: print(ch)
来源：http://mny.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tne.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hnd.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://aca.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yvi.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tum.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://fst.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yup.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://sku.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xpa.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://abm.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kcx.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://itk.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mty.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://urj.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tqy.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rze.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://xwq.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ufd.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ooh.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vyy.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cgv.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cfv.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bvu.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ruv.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ilf.yonumen.top

[E16] 数字千分位
来源：http://wmf.hammf.cn

Py:   f"{1234567:,}"
来源：http://kjx.zhengqikj.top

PHP:  number_format(1234567);
来源：http://cbq.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ngi.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://new.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vyr.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gsn.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://odh.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://dmx.zhixingplan.top

[E17] 首字母大写
来源：http://lhj.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uee.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kxv.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zaj.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cvs.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wnm.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ptu.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://wow.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mfs.hammf.cn

[E18] 模板占位符替换
来源：http://vdq.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mcg.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pwx.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://czc.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wbq.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xkq.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vow.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iij.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iqm.meibo888.top

[E19] 多行文本按行拆分
来源：http://hal.yuanzhike.top

Py:   s.splitlines()
来源：http://din.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lxa.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://kir.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://srn.zhiwuduotai.top

Java: s.lines().toList()
来源：http://spw.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://iih.jlsjyb.cn


<!-- 参考信息 -->