代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ztr.vqdsnc.cn

Go:   // 手写循环
来源：http://wvk.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://odd.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ayk.gaohongyu789.top

[D15] 去重
来源：http://rbj.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uah.yvedp.cn

PHP:  array_unique($arr);
来源：http://yrg.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://aju.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://kpv.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zob.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wpv.hysaishi.cn

Ruby: arr.uniq
来源：http://ewd.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://ykr.zdbjq.cn

[D16] 求和与平均值
来源：http://mql.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cvh.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aco.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dsx.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://erw.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://prk.nwbrower.top

Go:   // 手写循环累加
来源：http://rkg.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xcj.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://fah.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://yme.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://ibe.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://ytl.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uyd.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://wlm.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eru.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ngq.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://dnm.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://tor.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://kkk.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pqu.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://ern.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wfb.cheryme.top

TS:   nested.flat();
来源：http://rik.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://twd.smart0.xyz

Go:   // 手写双层循环
来源：http://arl.iojbl.cn

Ruby: nested.flatten
来源：http://fjn.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://haa.ydzc1.top

[D19] 按字段分组
来源：http://cnu.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iwy.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fdo.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ihn.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rwo.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qkn.tanke756.top

Go:   // 手写 map[string][]T
来源：http://drs.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://krv.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dad.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://dqr.guowangkeji.top

Py:   Counter(arr)
来源：http://kwl.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://nix.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgo.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwo.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://feb.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://hxq.ydjk.org.cn

Ruby: arr.tally
来源：http://tyv.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eic.meibo888.top

[D21] 判断是否包含某元素
来源：http://xap.dianchejie.cn

Py:   x in arr
来源：http://iri.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://owb.hysaishi.cn

JS:   arr.includes(x)
来源：http://ehg.hnqzz.top

TS:   arr.includes(x)
来源：http://bva.tianlin.xyz

Java: list.contains(x)
来源：http://twg.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://gtv.hywenlv.cn

Ruby: arr.include?(x)
来源：http://klu.ehwqpu.com

C#:   list.Contains(x)
来源：http://egk.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://wsk.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ipv.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jfr.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bpm.shanyushiyangtech.top

TS:   [...arr];
来源：http://thg.tian-w.cn

Java: new ArrayList<>(list);
来源：http://tym.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://khj.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://qpt.9152youxi.cn

C#:   new List<int>(list);
来源：http://aos.kuanghao11.cn

[D23] reduce 累积计算
来源：http://idc.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wuq.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dsp.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbh.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yqp.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://fkw.yj202588.top

Go:   // 手写循环
来源：http://vfn.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gtb.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ciu.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://jnn.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fot.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rqo.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://urr.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://btt.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ocn.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ymw.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mwo.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hya.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://sss.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jnb.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jyq.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ccl.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://szm.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sxf.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wsw.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://stm.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ocl.kuanghao11.cn

[D26] 数组转字符串
来源：http://bvo.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://cei.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://wxs.yj20258.top

JS:   arr.join(", ")
来源：http://xdd.hesvh.cn

TS:   arr.join(", ")
来源：http://ifu.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://fmh.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://xlu.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://iml.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://url.jlsjyb.cn

================================================================================
来源：http://dyv.daxiang520.top

E. 字符串处理
来源：http://zln.c1oappe.top

================================================================================
来源：http://asj.yangfankeji.com

[E01] 拼接字符串
来源：http://uae.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rpe.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ibo.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vme.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vog.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://idd.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sha.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hli.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgb.yj202588.top

[E02] 重复字符串
来源：http://fac.wangshuangyany.cn

Py:   "ab" * 3
来源：http://drf.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://zmk.yj20258.top

JS:   "ab".repeat(3)
来源：http://isj.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://kgt.xinyue.icu

Java: "ab".repeat(3)
来源：http://mut.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://vbg.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://mck.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://itj.nanxinkj.top

[E03] 截取子串
来源：http://vst.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mdy.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vea.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xqw.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://cpt.aibaodan.cn

Java: s.substring(1, 4)
来源：http://yzj.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vyz.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mru.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://kdn.kuanghao11.cn

[E04] 查找子串位置
来源：http://win.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://crz.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://ffq.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pcr.gotoacloud.top

TS:   s.indexOf("x")
来源：http://iho.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://cni.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://rca.zhijiandao.cn

Ruby: s.index("x")
来源：http://jmi.xziqi.cn

C#:   s.IndexOf("x")
来源：http://kiy.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://puw.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dcc.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bps.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://evw.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lsa.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcc.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hms.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xyk.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tcl.zhijiandao.cn

[E06] 替换子串
来源：http://avl.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qoc.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://gwj.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tgq.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ssi.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ycg.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dcr.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fyi.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://xck.9152youxi.cn

[E07] 按分隔符拆分
来源：http://uuy.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pqb.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lfu.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mqs.hfpthk.cn

TS:   s.split(",")
来源：http://tgy.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://yoa.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xmq.meibo888.top

Ruby: s.split(",");  s.split
来源：http://vom.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fmc.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://zyg.sweek.top

Py:   ",".join(items)
来源：http://cgh.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://mxo.jinqigufen.top

JS:   items.join(",")
来源：http://owd.cashguo.top

TS:   items.join(",")
来源：http://eyp.gaohongyu789.top

Java: String.join(",", items)
来源：http://zvb.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://int.xziqi.cn

Ruby: items.join(",")
来源：http://ztq.316326.xyz

C#:   string.Join(",", items)
来源：http://yqo.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://nbj.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ldr.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://paj.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://gnv.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://til.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://yar.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://afk.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://zin.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yzw.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://ezg.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ags.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qnl.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://fhe.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://qch.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://imx.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mcf.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://llu.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://odk.fanxiaobao.xyz

[E11] 反转字符串
来源：http://flj.xylfe.cn

Py:   s[::-1]
来源：http://lgp.zhiwuduotai.top

PHP:  strrev($s);
来源：http://nku.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://fak.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://pyd.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lxk.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qle.meibo888.top

Ruby: s.reverse
来源：http://pst.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://esp.xinyue.icu

[E12] 统计某字符出现次数
来源：http://rbj.dianchejie.cn

Py:   s.count("a")
来源：http://atx.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://lot.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://nfx.yj202588.top

TS:   s.split("a").length - 1
来源：http://hqm.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://trp.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://noa.shuidangran.top

Ruby: s.count("a")
来源：http://zxq.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://jas.xinyue.icu

[E13] 逐字符遍历
来源：http://zuz.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://hsq.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zjr.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oqd.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://sxt.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bza.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ygr.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://riz.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://duo.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://ahe.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kav.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://wmv.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://faw.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kdk.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bet.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nhg.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yuo.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kyw.sweek.top

[E15] HTML 转义 / 反转义
来源：http://sho.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bsa.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dpa.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mri.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://tgk.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ppi.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://htk.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vtj.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qma.hfpthk.cn

[E16] 数字千分位
来源：http://uvq.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://aff.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://ads.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://yoz.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aqj.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jsr.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://otq.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://shy.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://kpc.xylfe.cn

[E17] 首字母大写
来源：http://qji.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ezi.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fss.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aff.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://efj.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gps.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://obg.yuanzhike.top

Ruby: s.capitalize
来源：http://ies.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aez.xuanzx.com

[E18] 模板占位符替换
来源：http://sfc.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cun.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kik.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://szb.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hlm.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tlc.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pco.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aqb.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dxp.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://tgf.bjfxy.top

Py:   s.splitlines()
来源：http://avl.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rtz.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://utj.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://gws.sweek.top

Java: s.lines().toList()
来源：http://sug.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://waj.gaohongyu789.top

Ruby: s.lines
来源：http://tas.tarul.cn

C#:   s.Split('\n')
来源：http://ewa.fzhhl.top

[E20] 判断字符串是否为空
来源：http://nox.cqqwz.cn

Py:   if not s:
来源：http://voz.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://evk.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ddb.guowangkeji.top

TS:   if (s === "") {}
来源：http://och.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://jpv.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://qse.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://ggc.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pde.cdnleiting.top

[E21] 超长截断加省略号
来源：http://ecd.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://trq.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jtn.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xfm.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ajw.cucudq.cn


<!-- 参考信息 -->