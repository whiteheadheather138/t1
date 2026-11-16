代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfj.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xlj.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rte.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://vpn.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ytq.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://shh.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://smi.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://rgz.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dzb.tianlin.xyz

Go:   // 手写循环
来源：http://pdz.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xsw.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ndx.zhongyouzk.top

[D15] 去重
来源：http://lyv.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ryx.ppjwa.cn

PHP:  array_unique($arr);
来源：http://vmu.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://gsv.smart0.xyz

TS:   [...new Set(arr)]
来源：http://bsk.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hzu.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://gyr.zhixingplan.top

Ruby: arr.uniq
来源：http://ppv.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://dub.yongpay.top

[D16] 求和与平均值
来源：http://aqk.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rjo.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ezq.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jud.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hiy.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jfo.fehbvm.com

Go:   // 手写循环累加
来源：http://mrq.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://egg.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://mhq.fehbvm.com

[D17] 最大值与最小值
来源：http://chn.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://hdn.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://ieb.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rhi.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://yxf.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ppb.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fdh.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://jdi.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://tiw.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://jrl.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kxp.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://xbj.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uzs.yvedp.cn

TS:   nested.flat();
来源：http://gnm.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vjk.vqdsnc.cn

Go:   // 手写双层循环
来源：http://aax.jyoumei.cn

Ruby: nested.flatten
来源：http://tbh.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tzn.yj202588.top

[D19] 按字段分组
来源：http://gyb.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cnn.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rzf.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://smt.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://rru.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pxw.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://kil.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lho.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mov.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://auu.hnqzz.top

Py:   Counter(arr)
来源：http://rsk.52xcode.cn

PHP:  array_count_values($arr);
来源：http://vwv.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbf.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zra.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dyp.shuidangran.top

Go:   // 手写 map[T]int
来源：http://dhr.yueranfly.top

Ruby: arr.tally
来源：http://iig.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sgn.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://jtl.hfpthk.cn

Py:   x in arr
来源：http://fxw.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://tqk.sxryk.cn

JS:   arr.includes(x)
来源：http://nnn.chenlongwang.top

TS:   arr.includes(x)
来源：http://ctx.gogol.net.cn

Java: list.contains(x)
来源：http://bcc.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://pfv.tian-w.cn

Ruby: arr.include?(x)
来源：http://ona.gaohongyu789.top

C#:   list.Contains(x)
来源：http://mll.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://opu.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lgz.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cct.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nlj.yangfankeji.com

TS:   [...arr];
来源：http://bcn.yonumen.top

Java: new ArrayList<>(list);
来源：http://mnz.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://vwd.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://mgk.wangdashe.top

C#:   new List<int>(list);
来源：http://dht.tianlin.xyz

[D23] reduce 累积计算
来源：http://rwf.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wxz.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jts.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hwv.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkh.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sgg.daxiang520.top

Go:   // 手写循环
来源：http://yho.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ktm.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mps.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://cbh.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jsr.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fil.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pyx.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dfv.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tuu.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lwg.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lew.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ivf.316326.xyz

[D25] Set 集合去重与交并差
来源：http://wlt.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aka.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dyq.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mvb.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oxq.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ncq.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zrp.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xlv.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qmt.snrcjt.cn

[D26] 数组转字符串
来源：http://pxp.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://vgy.ivvv.top

PHP:  implode(", ", $arr);
来源：http://dzv.hnqzz.top

JS:   arr.join(", ")
来源：http://sjr.xylfe.cn

TS:   arr.join(", ")
来源：http://fjj.xziqi.cn

Java: String.join(", ", list)
来源：http://vjv.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://gur.hysaishi.cn

Ruby: arr.join(", ")
来源：http://syg.tarul.cn

C#:   string.Join(", ", list)
来源：http://rej.zhijiandao.cn

================================================================================
来源：http://pfa.hnxiangtu.top

E. 字符串处理
来源：http://jon.birdmap.top

================================================================================
来源：http://hpx.yangfankeji.com

[E01] 拼接字符串
来源：http://pjq.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://anh.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lov.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bof.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ffr.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ctb.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mlu.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qeh.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ltr.0kj1m.cn

[E02] 重复字符串
来源：http://kds.fzhhl.top

Py:   "ab" * 3
来源：http://ltt.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://gag.guannengcc.top

JS:   "ab".repeat(3)
来源：http://opk.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://upy.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://knv.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://wye.cqqwz.cn

Ruby: "ab" * 3
来源：http://ptt.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ams.vqdsnc.cn

[E03] 截取子串
来源：http://mvl.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pjz.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jzr.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xqb.uphjek.com

TS:   s.slice(1, 4)
来源：http://agz.hywenlv.cn

Java: s.substring(1, 4)
来源：http://doz.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dam.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://cib.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://zpf.birdmap.top

[E04] 查找子串位置
来源：http://bmm.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://gwa.gzhubu.top

PHP:  strpos($s, "x");
来源：http://lmc.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zlr.cucudq.cn

TS:   s.indexOf("x")
来源：http://xdd.c1oappe.top

Java: s.indexOf("x")
来源：http://yub.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://pdg.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://tqp.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://fhz.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://btb.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uiv.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rhb.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xom.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bij.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ljv.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pum.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubz.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fet.sweek.top

[E06] 替换子串
来源：http://lxv.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://flg.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://bsu.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://crx.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://yvn.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hab.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cld.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fxd.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://otw.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://qfh.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yae.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gjq.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hwy.hywenlv.cn

TS:   s.split(",")
来源：http://sln.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tww.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ozz.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://lrk.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gsu.shuidangran.top

[E08] 数组按分隔符合并
来源：http://kgd.bjfxy.top

Py:   ",".join(items)
来源：http://ntm.sxryk.cn

PHP:  implode(",", $items);
来源：http://uag.tianlin.xyz

JS:   items.join(",")
来源：http://rdh.zhengqikj.top

TS:   items.join(",")
来源：http://zpc.haohaochexian.top

Java: String.join(",", items)
来源：http://cod.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://rvr.nwbrower.top

Ruby: items.join(",")
来源：http://nvi.yuxming.cn

C#:   string.Join(",", items)
来源：http://soo.cqqwz.cn

[E09] 去除所有空白字符
来源：http://awp.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jln.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pya.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://qkm.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://taf.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://qih.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wem.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://upe.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqp.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://oyu.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iwj.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fvv.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://jzr.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://ikm.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://gkg.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wia.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xjp.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://llz.quarkkingdee.top

[E11] 反转字符串
来源：http://yhn.hysaishi.cn

Py:   s[::-1]
来源：http://naz.zhijiandao.cn

PHP:  strrev($s);
来源：http://icc.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://gay.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://xxo.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mdm.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gri.zhijiandao.cn

Ruby: s.reverse
来源：http://qmy.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xam.sysykeji.top

[E12] 统计某字符出现次数
来源：http://aen.jiagoushi.top

Py:   s.count("a")
来源：http://rvs.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://wca.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://lxp.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://zqt.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://irn.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://cdy.yangfankeji.com

Ruby: s.count("a")
来源：http://ydv.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://sit.cqqwz.cn

[E13] 逐字符遍历
来源：http://jkp.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://brm.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ugd.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://fxg.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ydp.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://agg.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jwf.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bbj.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fah.yuxming.cn

[E14] URL 编码与 Base64
来源：http://pql.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://otk.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qkp.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://shs.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mjs.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ifm.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vye.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qwh.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oxv.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://xqp.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://dgw.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fpr.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vel.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mdn.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wsr.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yah.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wlo.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dni.yongpay.top

[E16] 数字千分位
来源：http://vnh.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://jcj.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://yha.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://srv.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ygp.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://edk.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lmj.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tvu.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://vjk.52xcode.cn

[E17] 首字母大写
来源：http://jdu.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tjo.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://itj.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jgm.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ett.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xww.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iaz.zdbjq.cn

Ruby: s.capitalize
来源：http://jnp.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rjv.jianghu66.top

[E18] 模板占位符替换
来源：http://hqt.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fud.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nuy.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bpu.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ktu.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://prk.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://owb.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jea.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://elq.bbcook.cn

[E19] 多行文本按行拆分
来源：http://rqk.aizwys.cn

Py:   s.splitlines()
来源：http://pxm.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eyr.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://ccv.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://pcx.fktsv.cn

Java: s.lines().toList()
来源：http://ywi.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://ixi.shuidangran.top

Ruby: s.lines
来源：http://wlt.ctjpmb.com

C#:   s.Split('\n')
来源：http://nxa.xuanzx.com

[E20] 判断字符串是否为空
来源：http://sgo.jinqigufen.top

Py:   if not s:
来源：http://lzt.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://owy.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bgf.yuanzhike.top

TS:   if (s === "") {}
来源：http://uqn.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://nkw.wangshuangyany.cn


<!-- 参考信息 -->