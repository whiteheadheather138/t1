代发 wailian999

Ruby: arr.index(x)
来源：http://bzk.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://hoe.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://gcv.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sbj.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vnq.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://uju.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://qlq.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://skd.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ofi.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://bek.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ftb.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://cun.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xuo.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pdw.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://ora.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://qwy.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rod.ydjk.org.cn

Go:   // 手写循环
来源：http://wlh.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zxa.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://loo.chenzaomai.com

[D15] 去重
来源：http://rgz.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ksp.havefunace.top

PHP:  array_unique($arr);
来源：http://xbn.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://jnh.fengsongda.top

TS:   [...new Set(arr)]
来源：http://vtk.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vnw.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://jwx.cheryme.top

Ruby: arr.uniq
来源：http://aym.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://cku.kuanghao11.cn

[D16] 求和与平均值
来源：http://tbc.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqw.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rvi.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uzo.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lps.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gcw.zhengqikj.top

Go:   // 手写循环累加
来源：http://qol.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ecm.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://did.tanke756.top

[D17] 最大值与最小值
来源：http://lgj.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://tyn.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://ifl.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jsz.ppjwa.cn

TS:   Math.max(...arr);
来源：http://xwe.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kbn.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://usu.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://jqv.shangyingyoupin.top

C#:   list.Max();  list.Min()
来源：http://wxs.yj20258.top

[D18] 扁平化嵌套数组
来源：http://rki.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wna.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://hxm.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qbr.ydzc1.top

TS:   nested.flat();
来源：http://bdd.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tgf.tanke756.top

Go:   // 手写双层循环
来源：http://kzp.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://qfa.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ewj.ybcxt.top

[D19] 按字段分组
来源：http://bzu.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wdf.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xcc.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfa.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kag.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kuw.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://ujd.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://whf.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lub.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://gqp.fengsongda.top

Py:   Counter(arr)
来源：http://opi.iojbl.cn

PHP:  array_count_values($arr);
来源：http://aea.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aqz.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eba.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iym.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://lce.c1oappe.top

Ruby: arr.tally
来源：http://ven.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ztx.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://ivi.tanke756.top

Py:   x in arr
来源：http://iyf.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://utc.hammf.cn

JS:   arr.includes(x)
来源：http://gue.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://qlk.haohaochexian.top

Java: list.contains(x)
来源：http://evr.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://sho.ivvv.top

Ruby: arr.include?(x)
来源：http://tit.sweek.top

C#:   list.Contains(x)
来源：http://jqa.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://yao.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://owk.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mwb.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bni.cdnleiting.top

TS:   [...arr];
来源：http://stx.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://ljp.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://mxz.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://izo.jianghu66.top

C#:   new List<int>(list);
来源：http://qbh.kuanghao11.cn

[D23] reduce 累积计算
来源：http://wtx.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ite.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ivm.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://slw.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dyx.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dco.quarkkingdee.top

Go:   // 手写循环
来源：http://brh.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fdt.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pod.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://dav.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://enf.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vwh.gzhubu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mdt.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cfo.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yce.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vhn.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twr.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://woh.cheryme.top

[D25] Set 集合去重与交并差
来源：http://ulh.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ehl.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bkx.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kaa.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iyk.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dne.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tmd.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qnp.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yal.aizwys.cn

[D26] 数组转字符串
来源：http://bmg.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://zdu.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://ibo.gogol.net.cn

JS:   arr.join(", ")
来源：http://rqq.xinyue.icu

TS:   arr.join(", ")
来源：http://ntw.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://olf.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://ojm.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://rwk.smart0.xyz

C#:   string.Join(", ", list)
来源：http://jho.chenlongwang.top

================================================================================
来源：http://wgx.xinyue.icu

E. 字符串处理
来源：http://gje.tanke756.top

================================================================================
来源：http://vro.hammf.cn

[E01] 拼接字符串
来源：http://igi.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wyb.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qam.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvu.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dhr.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jhx.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uyp.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qss.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rbv.ehwqpu.com

[E02] 重复字符串
来源：http://fbm.svipenyu.cn

Py:   "ab" * 3
来源：http://hkh.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://mwu.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://ett.guannengcc.top

TS:   "ab".repeat(3)
来源：http://tkz.yj20258.top

Java: "ab".repeat(3)
来源：http://vby.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://pdo.epnwcf.com

Ruby: "ab" * 3
来源：http://ilo.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ifo.fengsongda.top

[E03] 截取子串
来源：http://ptt.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://icz.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ijc.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gvc.redwolf501.top

TS:   s.slice(1, 4)
来源：http://jeu.zhengqikj.top

Java: s.substring(1, 4)
来源：http://lyh.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aij.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ahu.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://dtq.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://nis.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://pei.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://btt.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vbh.birdmap.top

TS:   s.indexOf("x")
来源：http://nok.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://wtb.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://uys.shzxlz.cn

Ruby: s.index("x")
来源：http://tcs.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://caw.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qyu.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bkv.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zpp.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://asq.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iiq.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upd.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hja.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://euj.hywenlv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yhz.dashuyun.cn

[E06] 替换子串
来源：http://vja.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ort.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://ene.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://edk.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://eqn.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ssu.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dah.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://inz.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://qwv.c1oappe.top

[E07] 按分隔符拆分
来源：http://dxb.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bqh.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zsb.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://lcv.chenjidiqi.icu

TS:   s.split(",")
来源：http://ssf.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://sfo.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zuz.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://vcm.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kls.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://ypk.mhx1999.top

Py:   ",".join(items)
来源：http://puf.hfpthk.cn

PHP:  implode(",", $items);
来源：http://qrb.gogol.net.cn

JS:   items.join(",")
来源：http://eoo.tian-w.cn

TS:   items.join(",")
来源：http://jge.hongshengwenyu.top

Java: String.join(",", items)
来源：http://jzv.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://wyv.ivvv.top

Ruby: items.join(",")
来源：http://vse.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://xls.mhx1999.top

[E09] 去除所有空白字符
来源：http://qlr.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yct.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kip.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://gky.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://eop.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://bsz.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbw.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jqm.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oyu.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://tks.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cpj.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qma.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://ajn.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://bao.uphjek.com

Java: String.format("%03d", 7)
来源：http://ntj.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://bcb.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bou.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ett.zycfv.cn

[E11] 反转字符串
来源：http://aho.hysaishi.cn

Py:   s[::-1]
来源：http://rrw.wangshuangyany.cn

PHP:  strrev($s);
来源：http://wke.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://djb.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://vjw.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jsm.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zsh.hcnkem.com

Ruby: s.reverse
来源：http://qee.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bxq.sysykeji.top

[E12] 统计某字符出现次数
来源：http://aqq.hysaishi.cn

Py:   s.count("a")
来源：http://nvf.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://fsj.zycfv.cn

JS:   s.split("a").length - 1
来源：http://iio.yvedp.cn

TS:   s.split("a").length - 1
来源：http://yas.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iyh.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://til.yangfankeji.com

Ruby: s.count("a")
来源：http://rho.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://rjp.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://lnh.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://arc.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xzz.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://nef.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pzn.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oiz.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xsg.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lrs.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xqb.ybcxt.top

[E14] URL 编码与 Base64
来源：http://mlr.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pye.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://agv.52xcode.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://grq.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jhu.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xkj.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eiy.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tzz.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mwe.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://uvy.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://woc.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uql.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mbv.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lbe.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uak.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xjr.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cix.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oru.9152youxi.cn

[E16] 数字千分位
来源：http://ufe.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://srr.snrcjt.cn

PHP:  number_format(1234567);
来源：http://mhi.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://icm.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://leb.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dwv.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccd.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zfi.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://gsd.jianghu66.top

[E17] 首字母大写
来源：http://qei.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://exv.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyw.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uxd.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mjv.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jkb.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lna.yongpay.top

Ruby: s.capitalize
来源：http://iba.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ilj.mhx1999.top

[E18] 模板占位符替换
来源：http://vic.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yta.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kch.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mvx.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://umc.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mxk.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kyy.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nmj.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tgc.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://fpe.tianlin.xyz

Py:   s.splitlines()
来源：http://wqy.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wba.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://too.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://jhk.tanke756.top

Java: s.lines().toList()
来源：http://boj.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://adl.sxryk.cn


<!-- 参考信息 -->