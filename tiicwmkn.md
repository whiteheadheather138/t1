代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pkc.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://xgs.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://ohe.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://owl.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ord.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://sfs.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cus.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://fer.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://upc.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qrf.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://zpq.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://ohj.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://juc.cashguo.top

Go:   // 手写循环
来源：http://rnp.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://flu.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pqm.ivvv.top

[D15] 去重
来源：http://tts.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oyy.hammf.cn

PHP:  array_unique($arr);
来源：http://xwc.xziqi.cn

JS:   [...new Set(arr)]
来源：http://iih.hesvh.cn

TS:   [...new Set(arr)]
来源：http://bdt.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ptg.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://sfg.yvedp.cn

Ruby: arr.uniq
来源：http://etv.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://adi.hcnkem.com

[D16] 求和与平均值
来源：http://bzw.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ccm.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uhq.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://thw.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tqp.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ale.zhixingplan.top

Go:   // 手写循环累加
来源：http://zas.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://txd.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://rql.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://zxx.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://ldx.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://pnm.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://myp.xuanzx.com

TS:   Math.max(...arr);
来源：http://lat.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rtv.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nsq.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://vzv.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://qtg.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://kly.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hso.pycfn.com

PHP:  array_merge(...$nested);
来源：http://sbq.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fay.cqqwz.cn

TS:   nested.flat();
来源：http://cqm.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cof.cashguo.top

Go:   // 手写双层循环
来源：http://zvo.jiagoushi.top

Ruby: nested.flatten
来源：http://ukr.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgm.hongshengwenyu.top

[D19] 按字段分组
来源：http://dbf.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qvn.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://moa.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wom.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jkb.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nam.yj202588.top

Go:   // 手写 map[string][]T
来源：http://pcn.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wut.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://agu.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://mhh.vqdsnc.cn

Py:   Counter(arr)
来源：http://gpp.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://mye.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nxm.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bkb.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arw.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://bva.nanxuanxn.top

Ruby: arr.tally
来源：http://tuf.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fbx.birdmap.top

[D21] 判断是否包含某元素
来源：http://ljn.quarkkingdee.top

Py:   x in arr
来源：http://roa.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://mfl.cashguo.top

JS:   arr.includes(x)
来源：http://btn.jiagoushi.top

TS:   arr.includes(x)
来源：http://eit.zdbjq.cn

Java: list.contains(x)
来源：http://dcq.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://awh.yuxming.cn

Ruby: arr.include?(x)
来源：http://epi.smart0.xyz

C#:   list.Contains(x)
来源：http://jmx.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://iss.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yco.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lvr.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tck.tanke756.top

TS:   [...arr];
来源：http://pnk.mhx1999.top

Java: new ArrayList<>(list);
来源：http://iem.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lpb.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://xad.hcnkem.com

C#:   new List<int>(list);
来源：http://wmc.uphjek.com

[D23] reduce 累积计算
来源：http://hkd.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mok.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://paq.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pgl.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nrg.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ydw.snrcjt.cn

Go:   // 手写循环
来源：http://jpp.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mru.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://krw.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://hbp.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dty.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nwf.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jya.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nwt.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kcp.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mpf.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xbc.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dhi.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://oyg.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qmr.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tad.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gbo.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://muu.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wil.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dhc.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://boy.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hri.gogol.net.cn

[D26] 数组转字符串
来源：http://qvg.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://rgz.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://tlv.dianchejie.cn

JS:   arr.join(", ")
来源：http://wqn.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://gzl.bjfxy.top

Java: String.join(", ", list)
来源：http://euz.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://gdi.zdbjq.cn

Ruby: arr.join(", ")
来源：http://ocx.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://cwh.vehdjk.com

================================================================================
来源：http://rlt.chenzaomai.com

E. 字符串处理
来源：http://xzk.ydjk.org.cn

================================================================================
来源：http://ykj.gzhubu.top

[E01] 拼接字符串
来源：http://mjn.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tps.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hgu.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sku.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzz.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xcn.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vap.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pmt.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rvt.yuxming.cn

[E02] 重复字符串
来源：http://gff.fktsv.cn

Py:   "ab" * 3
来源：http://tpr.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://xqg.wangdashe.top

JS:   "ab".repeat(3)
来源：http://kgp.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://wzt.jyoumei.cn

Java: "ab".repeat(3)
来源：http://zoq.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://wzx.hnqzz.top

Ruby: "ab" * 3
来源：http://mdb.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://odx.chenjidiqi.icu

[E03] 截取子串
来源：http://qga.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vcg.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ful.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bpt.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://kzz.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://fxg.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tnw.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bfd.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://dqj.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://eoo.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://lig.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://kae.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jsy.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://kjl.hesvh.cn

Java: s.indexOf("x")
来源：http://xtz.tanke756.top

Go:   strings.Index(s, "x")
来源：http://akm.gzhubu.top

Ruby: s.index("x")
来源：http://vbs.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://gqw.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zci.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cwp.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zxh.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zew.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qff.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wjy.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pvl.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ykr.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ogs.nanxinkj.top

[E06] 替换子串
来源：http://izp.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ckv.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://dep.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://doc.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://bim.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pky.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://toe.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cqp.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://jqv.guowangkeji.top

[E07] 按分隔符拆分
来源：http://buf.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pno.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mrr.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nff.guannengcc.top

TS:   s.split(",")
来源：http://qvn.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://pqh.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sjf.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://yan.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xxn.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://dtf.xziqi.cn

Py:   ",".join(items)
来源：http://ktc.haohaochexian.top

PHP:  implode(",", $items);
来源：http://csv.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://ogo.chenzaomai.com

TS:   items.join(",")
来源：http://iyc.wangshuangyany.cn

Java: String.join(",", items)
来源：http://amh.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://dea.yangfankeji.com

Ruby: items.join(",")
来源：http://xng.cheryme.top

C#:   string.Join(",", items)
来源：http://wla.52xcode.cn

[E09] 去除所有空白字符
来源：http://jra.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zeg.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vwc.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://rxs.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://lqb.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://svw.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tor.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://xdc.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dzp.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://dkq.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tdq.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pqz.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://mtw.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://auc.gzhubu.top

Java: String.format("%03d", 7)
来源：http://aut.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hxd.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ork.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pxt.gaohongyu789.top

[E11] 反转字符串
来源：http://reh.hesvh.cn

Py:   s[::-1]
来源：http://qxl.yvedp.cn

PHP:  strrev($s);
来源：http://reu.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://dhw.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://slx.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ddu.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pyz.sweek.top

Ruby: s.reverse
来源：http://vlu.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rsu.hesvh.cn

[E12] 统计某字符出现次数
来源：http://syn.vqdsnc.cn

Py:   s.count("a")
来源：http://bay.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://ons.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://oqt.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://tev.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aye.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://mes.0kj1m.cn

Ruby: s.count("a")
来源：http://ckl.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://xyl.hysaishi.cn

[E13] 逐字符遍历
来源：http://swj.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://tpb.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwa.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hur.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jqt.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cti.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rkw.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pdi.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kvy.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://njg.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jwn.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xle.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ajp.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ebd.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qfc.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pds.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ljp.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fdn.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://bav.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://tpd.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kpb.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bii.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qyx.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rll.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gjx.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://afg.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ids.hesvh.cn

[E16] 数字千分位
来源：http://nus.cashguo.top

Py:   f"{1234567:,}"
来源：http://min.fktsv.cn

PHP:  number_format(1234567);
来源：http://gvm.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zvd.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://poz.tarul.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqd.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gyf.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dew.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://nuv.sufxvd.cn

[E17] 首字母大写
来源：http://oui.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oxy.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://myz.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qgg.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfx.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cth.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yzg.gotoacloud.top

Ruby: s.capitalize
来源：http://npm.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fel.zhijiandao.cn

[E18] 模板占位符替换
来源：http://vvn.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://elh.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iqt.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wko.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qgb.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijk.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://weh.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://twz.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://chb.316326.xyz

[E19] 多行文本按行拆分
来源：http://lyu.jqgfzy.top

Py:   s.splitlines()
来源：http://qzf.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://awp.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://tkm.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://bzj.shzxlz.cn

Java: s.lines().toList()
来源：http://nwd.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://jpe.chenzaomai.com

Ruby: s.lines
来源：http://npu.0kj1m.cn

C#:   s.Split('\n')
来源：http://kbk.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://hqd.cashguo.top

Py:   if not s:
来源：http://rbw.zhongyouzk.top


<!-- 参考信息 -->