代发 wailian999

Ruby: arr.index(x)
来源：http://ppi.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://gvk.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://pun.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sqe.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xjy.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://msa.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://axz.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jvm.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rak.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://mpl.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ams.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://tvi.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mzg.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pwe.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://nme.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://prk.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vkv.chenjidiqi.icu

Go:   // 手写循环
来源：http://nrt.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://cjm.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://qpp.dashuyun.cn

[D15] 去重
来源：http://ykp.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jma.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://bbo.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://hjq.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://vig.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ldu.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://bex.yvedp.cn

Ruby: arr.uniq
来源：http://hms.hammf.cn

C#:   list.Distinct().ToList()
来源：http://uuc.yj202588.top

[D16] 求和与平均值
来源：http://yrq.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hfd.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vrv.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jvh.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://imf.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fsc.fehbvm.com

Go:   // 手写循环累加
来源：http://cgv.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mqi.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://lra.jiagoushi.top

[D17] 最大值与最小值
来源：http://nuu.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://dlh.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://pww.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://syg.meibo888.top

TS:   Math.max(...arr);
来源：http://jmw.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ofy.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fmj.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://vyp.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://fmu.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://ycs.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ufx.ivvv.top

PHP:  array_merge(...$nested);
来源：http://uof.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://szi.ppjwa.cn

TS:   nested.flat();
来源：http://hcu.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fxj.vehdjk.com

Go:   // 手写双层循环
来源：http://cav.svipenyu.cn

Ruby: nested.flatten
来源：http://vtf.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qim.cdnleiting.top

[D19] 按字段分组
来源：http://rxp.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jlx.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sln.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://clt.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rre.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hpy.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://cxq.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://abs.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://auu.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://izk.shangyingyoupin.top

Py:   Counter(arr)
来源：http://hfb.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://gii.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://daj.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iix.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uqh.epnwcf.com

Go:   // 手写 map[T]int
来源：http://cql.dianchejie.cn

Ruby: arr.tally
来源：http://for.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cym.ivvv.top

[D21] 判断是否包含某元素
来源：http://yqo.tianlin.xyz

Py:   x in arr
来源：http://wys.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://khs.ctjpmb.com

JS:   arr.includes(x)
来源：http://pax.dashuyun.cn

TS:   arr.includes(x)
来源：http://khh.snrcjt.cn

Java: list.contains(x)
来源：http://rnz.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://xrg.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://wzx.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://hjk.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://ekt.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://urj.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kar.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oar.tian-w.cn

TS:   [...arr];
来源：http://fvw.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://nzf.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://mta.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://jlh.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://jph.meibo888.top

[D23] reduce 累积计算
来源：http://pms.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://htg.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gog.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwb.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pgq.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tnc.guannengcc.top

Go:   // 手写循环
来源：http://eph.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ovl.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lkk.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://pbv.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hfg.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wgp.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ddl.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lcj.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vhx.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vwc.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zer.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jpo.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://xel.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sor.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gxz.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mpm.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fgb.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gnc.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cyc.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ljg.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wtw.pycfn.com

[D26] 数组转字符串
来源：http://syl.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://ata.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://wwr.hnqzz.top

JS:   arr.join(", ")
来源：http://jee.yvedp.cn

TS:   arr.join(", ")
来源：http://nsq.yongpay.top

Java: String.join(", ", list)
来源：http://kja.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://mhg.ppjwa.cn

Ruby: arr.join(", ")
来源：http://nbb.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://msa.yj202588.top

================================================================================
来源：http://wgi.guannengcc.top

E. 字符串处理
来源：http://jno.ywan-chungtsiang.top

================================================================================
来源：http://enw.ydzc1.top

[E01] 拼接字符串
来源：http://gmh.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jms.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eph.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://svp.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztj.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gmo.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yns.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dkl.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uht.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://too.hongshengwenyu.top

Py:   "ab" * 3
来源：http://nek.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://fld.meibo888.top

JS:   "ab".repeat(3)
来源：http://pic.daxiang520.top

TS:   "ab".repeat(3)
来源：http://ihl.sufxvd.cn

Java: "ab".repeat(3)
来源：http://ddc.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://nia.316326.xyz

Ruby: "ab" * 3
来源：http://ifj.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsm.cqqwz.cn

[E03] 截取子串
来源：http://iwn.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rmf.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gak.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nmg.zycfv.cn

TS:   s.slice(1, 4)
来源：http://hcb.shzxlz.cn

Java: s.substring(1, 4)
来源：http://zxp.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wbg.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://olb.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://fce.sysykeji.top

[E04] 查找子串位置
来源：http://dfx.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://qcy.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://lym.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zmn.yongpay.top

TS:   s.indexOf("x")
来源：http://jru.ivvv.top

Java: s.indexOf("x")
来源：http://tje.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://sda.vqdsnc.cn

Ruby: s.index("x")
来源：http://dii.ivvv.top

C#:   s.IndexOf("x")
来源：http://fxz.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rom.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yxp.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ads.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dar.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kdv.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hou.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tbk.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zem.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mlq.ppjwa.cn

[E06] 替换子串
来源：http://feo.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fxj.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://jaw.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aan.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://bdd.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xah.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hhx.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tca.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://khc.ctjpmb.com

[E07] 按分隔符拆分
来源：http://iuf.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyv.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ajx.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://adj.yuxming.cn

TS:   s.split(",")
来源：http://zqk.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ucr.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dkf.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://oki.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://awy.fktsv.cn

[E08] 数组按分隔符合并
来源：http://ywe.andypj.xyz

Py:   ",".join(items)
来源：http://ogf.gzhubu.top

PHP:  implode(",", $items);
来源：http://ttv.jiagoushi.top

JS:   items.join(",")
来源：http://egc.cucudq.cn

TS:   items.join(",")
来源：http://gyq.hysaishi.cn

Java: String.join(",", items)
来源：http://pug.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://nyn.shzxlz.cn

Ruby: items.join(",")
来源：http://wff.nanxinkj.top

C#:   string.Join(",", items)
来源：http://vas.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://sqi.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://adn.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ktg.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://yda.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://zlj.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://qjo.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ukz.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://vtn.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lbn.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://uoa.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oge.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hfg.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://eyz.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://nhw.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://ffc.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://jtg.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pzp.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yiz.cqqwz.cn

[E11] 反转字符串
来源：http://hyw.kuanghao11.cn

Py:   s[::-1]
来源：http://nbs.xziqi.cn

PHP:  strrev($s);
来源：http://khe.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://pkz.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://vmc.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gas.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zqj.bbcook.cn

Ruby: s.reverse
来源：http://ref.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jtl.cashguo.top

[E12] 统计某字符出现次数
来源：http://nne.shuidangran.top

Py:   s.count("a")
来源：http://bps.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://nod.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://php.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://bcf.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://amz.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://vky.chenjidiqi.icu

Ruby: s.count("a")
来源：http://nop.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://vjk.ehwqpu.com

[E13] 逐字符遍历
来源：http://pua.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://dom.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hhz.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ekh.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hpd.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ror.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://swt.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hae.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gif.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://kzv.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ert.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dsk.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jna.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jsd.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zhq.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://urg.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jhd.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mda.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://mnv.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://plg.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qft.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://png.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nbm.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fnw.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gsr.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uhv.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dvy.vehdjk.com

[E16] 数字千分位
来源：http://sot.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://eev.epnwcf.com

PHP:  number_format(1234567);
来源：http://zgr.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://irr.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dee.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kec.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://woq.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://agz.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://pdf.daxiang520.top

[E17] 首字母大写
来源：http://zjm.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lsq.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xsq.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jvm.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gfp.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qzd.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sci.mhx1999.top

Ruby: s.capitalize
来源：http://vuu.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tep.cqqwz.cn

[E18] 模板占位符替换
来源：http://lps.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vnm.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dff.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dkj.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://exj.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ryr.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lpm.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fpq.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://inc.birdmap.top

[E19] 多行文本按行拆分
来源：http://dwx.ehwqpu.com

Py:   s.splitlines()
来源：http://bgb.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pbf.sweek.top

JS:   s.split(/\r?\n/)
来源：http://ske.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://zwy.jqgufenzy.top

Java: s.lines().toList()
来源：http://kcj.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://wmy.smart0.xyz


<!-- 参考信息 -->