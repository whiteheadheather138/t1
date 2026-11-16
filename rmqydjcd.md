代发 wailian999

TS:   [...new Set(arr)]
来源：http://ozj.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dsy.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qkm.0kj1m.cn

Ruby: arr.uniq
来源：http://xyy.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://nag.jyoumei.cn

[D16] 求和与平均值
来源：http://ivd.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vaj.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ban.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://enn.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://prz.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aiy.ydjk.org.cn

Go:   // 手写循环累加
来源：http://lao.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pgo.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://otk.fzhhl.top

[D17] 最大值与最小值
来源：http://rut.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://vid.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://mbe.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://erx.pycfn.com

TS:   Math.max(...arr);
来源：http://chm.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fxc.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wii.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://glt.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://mgk.pycfn.com

[D18] 扁平化嵌套数组
来源：http://xoa.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dba.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://bxb.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lkm.ppjwa.cn

TS:   nested.flat();
来源：http://psw.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yrl.yj20258888.top

Go:   // 手写双层循环
来源：http://jab.feifeiyinyue.top

Ruby: nested.flatten
来源：http://bzg.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mbw.vqdsnc.cn

[D19] 按字段分组
来源：http://mgd.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ort.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vba.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vfc.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rbz.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zil.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://eox.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tiy.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vtr.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://ijb.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://hex.ybcxt.top

PHP:  array_count_values($arr);
来源：http://ort.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ddj.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nsh.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cpx.sysykeji.top

Go:   // 手写 map[T]int
来源：http://gdk.ctjpmb.com

Ruby: arr.tally
来源：http://xgd.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qgk.hcnkem.com

[D21] 判断是否包含某元素
来源：http://oue.kuanghao11.cn

Py:   x in arr
来源：http://xmr.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://puj.zhixingplan.top

JS:   arr.includes(x)
来源：http://lbo.yongpay.top

TS:   arr.includes(x)
来源：http://yio.yvedp.cn

Java: list.contains(x)
来源：http://wfq.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://mzy.shuidangran.top

Ruby: arr.include?(x)
来源：http://guf.yongpay.top

C#:   list.Contains(x)
来源：http://rvo.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://eok.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://skr.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bkw.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lqv.316326.xyz

TS:   [...arr];
来源：http://vfn.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://xkj.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://lbf.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://lzd.zhengqikj.top

C#:   new List<int>(list);
来源：http://mbq.jinqigufen.top

[D23] reduce 累积计算
来源：http://zco.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qxv.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bhl.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vur.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eiw.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fqf.c1oappe.top

Go:   // 手写循环
来源：http://mea.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zqr.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://crw.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://uti.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ggr.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://onk.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jzf.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ecz.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nth.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkg.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ywg.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rsb.pycfn.com

[D25] Set 集合去重与交并差
来源：http://dcv.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wxh.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hem.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ehu.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jge.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txc.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://emb.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://szk.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kcn.mhx1999.top

[D26] 数组转字符串
来源：http://zza.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://dpq.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://hwl.jqgfzy.top

JS:   arr.join(", ")
来源：http://tbu.zhoulong.xyz

TS:   arr.join(", ")
来源：http://lmp.tianlin.xyz

Java: String.join(", ", list)
来源：http://uut.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://mro.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://exh.ybcxt.top

C#:   string.Join(", ", list)
来源：http://buo.svipenyu.cn

================================================================================
来源：http://vkk.gaohongyu789.top

E. 字符串处理
来源：http://bpg.zhijiandao.cn

================================================================================
来源：http://nul.vehdjk.com

[E01] 拼接字符串
来源：http://hfg.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bci.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ykx.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dtl.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wku.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xbi.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://slv.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://afx.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zcy.nwbrower.top

[E02] 重复字符串
来源：http://nvc.yj202588.top

Py:   "ab" * 3
来源：http://grk.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://jye.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://nsj.xylfe.cn

TS:   "ab".repeat(3)
来源：http://pme.pycfn.com

Java: "ab".repeat(3)
来源：http://loe.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://zhg.iojbl.cn

Ruby: "ab" * 3
来源：http://njm.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uhf.bjfxy.top

[E03] 截取子串
来源：http://lnu.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jpy.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ojf.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zxo.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://lll.jinqigufen.top

Java: s.substring(1, 4)
来源：http://pwa.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://byf.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rav.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://yqi.hcnkem.com

[E04] 查找子串位置
来源：http://svk.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://rte.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://zpa.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hzj.sweek.top

TS:   s.indexOf("x")
来源：http://ovq.haohaochexian.top

Java: s.indexOf("x")
来源：http://ows.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://rpj.guowangkeji.top

Ruby: s.index("x")
来源：http://nit.yvedp.cn

C#:   s.IndexOf("x")
来源：http://dch.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rxz.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lrz.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yqa.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ggd.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qnk.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcs.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://otf.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://asp.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tck.jinyuanbaomall.cn

[E06] 替换子串
来源：http://gvx.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vrm.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://yrk.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tdg.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://sgj.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kve.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eft.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://obo.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://ysc.jqgfzy.top

[E07] 按分隔符拆分
来源：http://teb.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sxz.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yqa.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://guk.haohaochexian.top

TS:   s.split(",")
来源：http://azs.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jkt.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://trq.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://nig.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://chj.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://vuw.zhoulong.xyz

Py:   ",".join(items)
来源：http://uid.pycfn.com

PHP:  implode(",", $items);
来源：http://wct.jinghuilouyu.cn

JS:   items.join(",")
来源：http://hyu.yvedp.cn

TS:   items.join(",")
来源：http://qxd.sweek.top

Java: String.join(",", items)
来源：http://vkf.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://obs.sysykeji.top

Ruby: items.join(",")
来源：http://odw.hysaishi.cn

C#:   string.Join(",", items)
来源：http://epv.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://huk.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vzq.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hhz.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://iua.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://meq.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://lpt.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oqz.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://tmv.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tin.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://wmy.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dao.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pca.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://byc.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://gui.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://csf.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yoo.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uvf.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fbv.jinghuilouyu.cn

[E11] 反转字符串
来源：http://yjh.ivvv.top

Py:   s[::-1]
来源：http://ikw.fehbvm.com

PHP:  strrev($s);
来源：http://xyu.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://jwa.tanke756.top

TS:   [...s].reverse().join("")
来源：http://qbd.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ewd.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jlo.kuanghao11.cn

Ruby: s.reverse
来源：http://xjh.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://xes.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://rtl.chenzaomai.com

Py:   s.count("a")
来源：http://rsx.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://kgk.cucudq.cn

JS:   s.split("a").length - 1
来源：http://mpp.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://jku.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gex.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://flf.birdmap.top

Ruby: s.count("a")
来源：http://fuk.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://gbs.uphjek.com

[E13] 逐字符遍历
来源：http://qmx.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://blg.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nug.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hcj.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wjo.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ett.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gbl.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ebk.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vkm.yj20258888.top

[E14] URL 编码与 Base64
来源：http://qyr.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://igh.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jly.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uhn.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cqf.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fhj.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bvm.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gai.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jnj.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://hdp.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://umr.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ked.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ceo.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fdx.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lun.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mns.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wyb.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eny.mhx1999.top

[E16] 数字千分位
来源：http://fpn.fengsongda.top

Py:   f"{1234567:,}"
来源：http://cmr.tianlin.xyz

PHP:  number_format(1234567);
来源：http://xuh.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xdd.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mrw.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jlh.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qfa.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fbi.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://bwa.gogol.net.cn

[E17] 首字母大写
来源：http://doe.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mee.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://osb.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hek.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yab.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://phz.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nip.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://qfp.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://noq.iojbl.cn

[E18] 模板占位符替换
来源：http://qho.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wyk.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kwa.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lgn.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hwl.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zsc.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yfc.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qkx.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dsk.redwolf501.top

[E19] 多行文本按行拆分
来源：http://jgp.bbcook.cn

Py:   s.splitlines()
来源：http://kun.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oat.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://jha.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://bbk.nanxuanxn.top

Java: s.lines().toList()
来源：http://zoc.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://akp.havefunace.top

Ruby: s.lines
来源：http://sgh.xuanzx.com

C#:   s.Split('\n')
来源：http://ggh.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://moa.gaohongyu789.top

Py:   if not s:
来源：http://okf.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pru.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xps.zhongyouzk.top

TS:   if (s === "") {}
来源：http://ygu.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://zbb.cqqwz.cn

Go:   if s == "" {}
来源：http://siz.ybcxt.top

Ruby: if s.empty?
来源：http://xno.hesvh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yex.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://oop.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ogr.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rju.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsj.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xdu.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bal.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://iiw.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sbz.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ahs.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://uow.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://asy.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ffv.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qay.tian-w.cn


<!-- 参考信息 -->