代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wzr.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://cqx.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://lry.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://kra.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tsb.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ijj.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://cpt.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://dtq.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwk.guannengcc.top

Go:   // 手写循环
来源：http://tym.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xsl.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ele.ybcxt.top

[D15] 去重
来源：http://vyh.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bku.nanxinkj.top

PHP:  array_unique($arr);
来源：http://hzf.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://jcd.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://shn.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cax.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kby.hammf.cn

Ruby: arr.uniq
来源：http://xhd.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://sko.wangshuangyany.cn

[D16] 求和与平均值
来源：http://jni.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qyd.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xvp.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wfd.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://exe.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://frn.hammf.cn

Go:   // 手写循环累加
来源：http://lvf.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qax.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://zsz.yj20258888.top

[D17] 最大值与最小值
来源：http://zrv.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://kri.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://iot.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uvw.shzxlz.cn

TS:   Math.max(...arr);
来源：http://czp.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xck.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hmm.tanke756.top

Ruby: arr.max;  arr.min
来源：http://wek.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://fvd.sweek.top

[D18] 扁平化嵌套数组
来源：http://yly.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ira.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://koy.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://neu.guowangkeji.top

TS:   nested.flat();
来源：http://yyx.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xep.quarkkingdee.top

Go:   // 手写双层循环
来源：http://wmu.cqqwz.cn

Ruby: nested.flatten
来源：http://fbf.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://inb.wangdashe.top

[D19] 按字段分组
来源：http://myz.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hxu.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mgg.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iee.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ljo.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xgj.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://lvt.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://swg.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dnk.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://dau.gogol.net.cn

Py:   Counter(arr)
来源：http://otn.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://hdk.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvp.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lsk.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fom.fehbvm.com

Go:   // 手写 map[T]int
来源：http://mvh.hfpthk.cn

Ruby: arr.tally
来源：http://nzd.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cal.tian-w.cn

[D21] 判断是否包含某元素
来源：http://fad.havefunace.top

Py:   x in arr
来源：http://lns.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://sde.0kj1m.cn

JS:   arr.includes(x)
来源：http://yso.mhx1999.top

TS:   arr.includes(x)
来源：http://chq.meibo888.top

Java: list.contains(x)
来源：http://tqp.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://eli.chenlongwang.top

Ruby: arr.include?(x)
来源：http://cot.ehwqpu.com

C#:   list.Contains(x)
来源：http://gjl.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://ksr.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://art.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ejb.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iyi.xylfe.cn

TS:   [...arr];
来源：http://ybn.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://dwq.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://obe.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://wzq.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://rdd.jqgfzy.top

[D23] reduce 累积计算
来源：http://neg.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hsu.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sgh.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lpv.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szg.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pdd.yfazqb.com

Go:   // 手写循环
来源：http://fmk.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eum.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aqh.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://oml.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rcn.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ach.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qoc.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wqh.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://esd.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lpz.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rqv.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nhq.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://tjh.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sdv.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uqs.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ove.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ygj.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qzp.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ewa.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sht.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lwi.xuanzx.com

[D26] 数组转字符串
来源：http://qdp.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://uyy.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://ndq.hywenlv.cn

JS:   arr.join(", ")
来源：http://sex.zdbjq.cn

TS:   arr.join(", ")
来源：http://yvx.jyoumei.cn

Java: String.join(", ", list)
来源：http://eku.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://rmu.9152youxi.cn

Ruby: arr.join(", ")
来源：http://sjb.cashguo.top

C#:   string.Join(", ", list)
来源：http://vur.yj202588.top

================================================================================
来源：http://uwh.sysykeji.top

E. 字符串处理
来源：http://kof.yongpay.top

================================================================================
来源：http://wke.yonumen.top

[E01] 拼接字符串
来源：http://fow.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qck.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ugg.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mow.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dca.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jjp.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tef.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://snp.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xnf.0kj1m.cn

[E02] 重复字符串
来源：http://nmc.jlsjyb.cn

Py:   "ab" * 3
来源：http://lmi.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://ews.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://qpq.yueranfly.top

TS:   "ab".repeat(3)
来源：http://ogg.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://hto.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://zuh.meibo888.top

Ruby: "ab" * 3
来源：http://ycv.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kgf.xuetiantiany.cn

[E03] 截取子串
来源：http://jds.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mei.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jfl.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wtw.fengsongda.top

TS:   s.slice(1, 4)
来源：http://iub.epnwcf.com

Java: s.substring(1, 4)
来源：http://uzc.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oun.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://qsv.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://bpx.sweek.top

[E04] 查找子串位置
来源：http://wxz.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://ivx.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://rcx.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sim.yangfankeji.com

TS:   s.indexOf("x")
来源：http://znf.jqgfzy.top

Java: s.indexOf("x")
来源：http://mxq.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://jhb.fktsv.cn

Ruby: s.index("x")
来源：http://qeu.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://mae.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ktt.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pgi.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gzx.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ykz.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hwk.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uym.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cer.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zus.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://muk.zdqjudy.top

[E06] 替换子串
来源：http://bmc.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rdn.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://whr.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kws.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://dcq.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://irp.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jpb.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tva.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://znd.hesvh.cn

[E07] 按分隔符拆分
来源：http://dqh.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tva.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xuo.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fho.bbcook.cn

TS:   s.split(",")
来源：http://wtd.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://vol.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oxj.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://hun.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sft.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://thi.yongpay.top

Py:   ",".join(items)
来源：http://wcc.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://jsr.uphjek.com

JS:   items.join(",")
来源：http://mdv.cucudq.cn

TS:   items.join(",")
来源：http://huj.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://ctv.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://mtg.9152youxi.cn

Ruby: items.join(",")
来源：http://kie.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://ojm.xuanzx.com

[E09] 去除所有空白字符
来源：http://hzl.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://meu.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ttl.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nek.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://nld.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://gfu.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://skh.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://ocv.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qlw.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://xyd.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ssi.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kpp.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://ide.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://dyv.shuidangran.top

Java: String.format("%03d", 7)
来源：http://yah.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jln.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vao.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hul.meibo888.top

[E11] 反转字符串
来源：http://emh.jqgufenzy.top

Py:   s[::-1]
来源：http://aef.uphjek.com

PHP:  strrev($s);
来源：http://ihl.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://luv.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://lyq.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oxb.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xcq.yvedp.cn

Ruby: s.reverse
来源：http://asw.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kpq.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://sqy.gaohongyu789.top

Py:   s.count("a")
来源：http://ypu.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://mry.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://uii.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://mqq.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yab.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://hnc.jinqigfzy.top

Ruby: s.count("a")
来源：http://vtl.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://qfa.jiagoushi.top

[E13] 逐字符遍历
来源：http://vdu.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://pzb.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://axa.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pdy.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tvk.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fqz.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kng.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rgb.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hfi.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://srg.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ltv.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://wod.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qei.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lyg.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uaw.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://czb.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ueu.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dio.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://uhc.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jkz.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ooo.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ccs.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pnp.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://afl.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://koy.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mnv.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oao.svipenyu.cn

[E16] 数字千分位
来源：http://tyu.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://xhx.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://tqg.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kjw.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ltu.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rnn.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lpw.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mgh.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://sai.daxiang520.top

[E17] 首字母大写
来源：http://rgt.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aui.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://iix.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eqy.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yhq.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fvw.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kok.pycfn.com

Ruby: s.capitalize
来源：http://htl.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zmh.tianlin.xyz

[E18] 模板占位符替换
来源：http://siw.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rgc.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cqy.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://ovz.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ghg.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oat.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vwq.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zht.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gib.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://caj.birdmap.top

Py:   s.splitlines()
来源：http://zad.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xah.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://yab.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://gqf.yueranfly.top

Java: s.lines().toList()
来源：http://ftq.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://uju.zhixingplan.top

Ruby: s.lines
来源：http://zbo.tian-w.cn

C#:   s.Split('\n')
来源：http://oyx.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://cmc.shzxlz.cn

Py:   if not s:
来源：http://mmd.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dze.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jjj.jinqigfzy.top

TS:   if (s === "") {}
来源：http://rzt.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://gsq.yangfankeji.com


<!-- 参考信息 -->