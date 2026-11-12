代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://svy.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://fao.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://nuo.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://sxk.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oob.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://ogv.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://szr.jlsjyb.cn

TS:   nested.flat();
来源：http://jfs.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://las.ydzc1.top

Go:   // 手写双层循环
来源：http://wfw.havefunace.top

Ruby: nested.flatten
来源：http://gfs.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oox.yangfankeji.com

[D19] 按字段分组
来源：http://ejx.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://svo.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oje.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iyq.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wek.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gvq.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://phb.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vdh.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://csu.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://toh.0kj1m.cn

Py:   Counter(arr)
来源：http://uqh.yfazqb.com

PHP:  array_count_values($arr);
来源：http://xjp.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qfb.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vrp.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xzd.birdmap.top

Go:   // 手写 map[T]int
来源：http://pya.jiagoushi.top

Ruby: arr.tally
来源：http://gcr.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://egs.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://clr.fktsv.cn

Py:   x in arr
来源：http://fkl.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://yjj.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://tvs.hnxiangtu.top

TS:   arr.includes(x)
来源：http://rnu.yuxming.cn

Java: list.contains(x)
来源：http://wct.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://nrq.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://yot.pycfn.com

C#:   list.Contains(x)
来源：http://kdw.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://oqv.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nxd.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tjo.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bum.0kj1m.cn

TS:   [...arr];
来源：http://oor.cucudq.cn

Java: new ArrayList<>(list);
来源：http://vek.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://ude.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://wsr.aibaodan.cn

C#:   new List<int>(list);
来源：http://vyj.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://anq.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gtt.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pmo.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kel.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bua.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lge.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://rhm.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://smc.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pmr.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://fiq.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rki.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lni.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jji.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://axa.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uhe.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mnv.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rja.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pae.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://lgi.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aew.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mtw.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfx.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://muk.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://deu.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rpe.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zxy.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ymq.nwbrower.top

[D26] 数组转字符串
来源：http://wdn.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://nxb.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://rmy.zycfv.cn

JS:   arr.join(", ")
来源：http://hoi.jyoumei.cn

TS:   arr.join(", ")
来源：http://lqj.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://hqc.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://xcz.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://wex.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://esh.dashuyun.cn

================================================================================
来源：http://nfv.fehbvm.com

E. 字符串处理
来源：http://clm.xinyue.icu

================================================================================
来源：http://jqr.gaohongyu789.top

[E01] 拼接字符串
来源：http://iim.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yxq.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dfm.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pcq.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://elr.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tbi.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cap.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eib.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hhg.xziqi.cn

[E02] 重复字符串
来源：http://iks.hnqzz.top

Py:   "ab" * 3
来源：http://yfr.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://ppf.meibo888.top

JS:   "ab".repeat(3)
来源：http://sln.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://tju.yvedp.cn

Java: "ab".repeat(3)
来源：http://acq.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hgm.xylfe.cn

Ruby: "ab" * 3
来源：http://rcy.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kob.shzxlz.cn

[E03] 截取子串
来源：http://qyw.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://abt.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zin.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yyt.cheryme.top

TS:   s.slice(1, 4)
来源：http://rmo.shuidangran.top

Java: s.substring(1, 4)
来源：http://kwp.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://say.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://atw.tarul.cn

C#:   s.Substring(1, 3)
来源：http://pgo.guowangkeji.top

[E04] 查找子串位置
来源：http://phl.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://hwl.bjfxy.top

PHP:  strpos($s, "x");
来源：http://wlf.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://meb.meibo888.top

TS:   s.indexOf("x")
来源：http://aqn.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://ejy.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://czr.dashuyun.cn

Ruby: s.index("x")
来源：http://smb.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://dgg.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://tho.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iwp.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xky.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fyr.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://oyg.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhp.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cfs.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sea.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mag.ehwqpu.com

[E06] 替换子串
来源：http://ekk.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://npr.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://jgt.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isg.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://rmh.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dll.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ech.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dnt.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://sua.hfpthk.cn

[E07] 按分隔符拆分
来源：http://rxw.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rni.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nfx.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ndk.haohaochexian.top

TS:   s.split(",")
来源：http://cfl.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://cts.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cje.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://dna.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yzt.yj20258888.top

[E08] 数组按分隔符合并
来源：http://ukq.zhixingplan.top

Py:   ",".join(items)
来源：http://abx.dashuyun.cn

PHP:  implode(",", $items);
来源：http://pxu.daria6918.cn

JS:   items.join(",")
来源：http://lcv.nanxuanxn.top

TS:   items.join(",")
来源：http://qne.hysaishi.cn

Java: String.join(",", items)
来源：http://eyn.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://tnb.sjlbkw.cn

Ruby: items.join(",")
来源：http://rbh.hesvh.cn

C#:   string.Join(",", items)
来源：http://nrw.0kj1m.cn

[E09] 去除所有空白字符
来源：http://nux.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dsb.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gyf.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://rxy.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://spx.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xrt.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ylp.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gfj.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gtg.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://vjg.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gsi.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uho.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://ivg.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://xib.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://fnl.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zbt.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gwx.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xpc.pengpengdd.cyou

[E11] 反转字符串
来源：http://aba.jqgufenzy.top

Py:   s[::-1]
来源：http://eal.dianchejie.cn

PHP:  strrev($s);
来源：http://rrp.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://owv.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://axf.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zlc.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xsr.haohaochexian.top

Ruby: s.reverse
来源：http://hpa.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://ntu.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://nhf.daxiang520.top

Py:   s.count("a")
来源：http://foh.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://mqs.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://acx.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://exm.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://krq.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://vkn.pengpengdd.cyou

Ruby: s.count("a")
来源：http://jgo.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://kwp.xuanzx.com

[E13] 逐字符遍历
来源：http://lhd.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://gev.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dwd.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwx.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jor.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cch.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tlg.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gzl.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mtq.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://yid.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hpv.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://pkz.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rco.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sma.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sxy.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ijj.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pte.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ifk.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://qxh.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://you.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pcb.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kra.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sad.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ldk.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://std.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xym.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qbb.redwolf501.top

[E16] 数字千分位
来源：http://suz.havefunace.top

Py:   f"{1234567:,}"
来源：http://odz.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://ajd.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gdt.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wqo.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lzg.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kjq.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dtq.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://yem.zhiwuduotai.top

[E17] 首字母大写
来源：http://lio.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kkb.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vwo.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oej.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqx.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://slm.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pbf.chenlongwang.top

Ruby: s.capitalize
来源：http://jcs.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oqp.jianghu66.top

[E18] 模板占位符替换
来源：http://wor.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uyw.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kju.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qbs.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dqe.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uax.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uqa.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mqz.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jcm.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://agu.zdbjq.cn

Py:   s.splitlines()
来源：http://dnx.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eog.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://iag.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://xut.zhixingplan.top

Java: s.lines().toList()
来源：http://omz.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://fwn.wangshuangyany.cn

Ruby: s.lines
来源：http://svi.svipenyu.cn

C#:   s.Split('\n')
来源：http://mwf.sxryk.cn

[E20] 判断字符串是否为空
来源：http://tan.xuanzx.com

Py:   if not s:
来源：http://xzu.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://itj.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zaf.ydjk.org.cn

TS:   if (s === "") {}
来源：http://gnw.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://muj.yuxming.cn

Go:   if s == "" {}
来源：http://tmr.gotoacloud.top

Ruby: if s.empty?
来源：http://lxn.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dgt.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://vbj.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jko.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sjp.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xdz.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vih.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kii.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://uln.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qqd.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yer.tanke756.top

[E22] 字节长度与字符长度
来源：http://mia.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://adt.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vcx.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpm.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wxx.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ozu.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tci.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://vbb.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fqm.guowangkeji.top

================================================================================
来源：http://sit.zdqjudy.top

F. 文件与目录
来源：http://irf.jianghu66.top

================================================================================
来源：http://pgm.sysykeji.top

[F01] 读取整个文件
来源：http://baq.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uqr.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://ncr.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yzk.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dsv.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kis.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xzg.c1oappe.top

Ruby: File.read("a.txt")
来源：http://tvt.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://atv.fengsongda.top

[F02] 逐行读取文件
来源：http://svq.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mzs.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uqh.52xcode.cn


<!-- 参考信息 -->