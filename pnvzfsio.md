代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zby.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://iqw.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://kaj.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://zzx.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fmq.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://tta.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xoo.shangyingyoupin.top

TS:   nested.flat();
来源：http://ihk.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fcx.dashuyun.cn

Go:   // 手写双层循环
来源：http://wcx.zdqjudy.top

Ruby: nested.flatten
来源：http://egq.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://kka.jinqigfzy.top

[D19] 按字段分组
来源：http://zgo.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://geg.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gbv.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ijy.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kzg.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://osk.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://nny.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pxt.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbp.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://vqf.pengpengdd.cyou

Py:   Counter(arr)
来源：http://iqc.xziqi.cn

PHP:  array_count_values($arr);
来源：http://eqv.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ppq.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwt.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qbq.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://qyu.316326.xyz

Ruby: arr.tally
来源：http://vte.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ljo.xuanzx.com

[D21] 判断是否包含某元素
来源：http://bla.fktsv.cn

Py:   x in arr
来源：http://lpt.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://tii.ydzc1.top

JS:   arr.includes(x)
来源：http://huh.zhoulong.xyz

TS:   arr.includes(x)
来源：http://bsq.ivvv.top

Java: list.contains(x)
来源：http://kgb.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://mep.daria6918.cn

Ruby: arr.include?(x)
来源：http://pga.fehbvm.com

C#:   list.Contains(x)
来源：http://tjh.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://prj.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lnm.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zyc.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ccf.gzhubu.top

TS:   [...arr];
来源：http://fjn.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://khe.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://jue.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://vxg.zdqjudy.top

C#:   new List<int>(list);
来源：http://ewp.0kj1m.cn

[D23] reduce 累积计算
来源：http://wpv.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://stq.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dnm.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzv.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yas.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://urm.316326.xyz

Go:   // 手写循环
来源：http://ezc.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blr.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vxs.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://xln.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rdt.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yav.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xpw.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tla.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://izf.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dlj.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xro.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dcg.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://jgl.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pzs.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sfk.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gic.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bpq.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uym.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://odi.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jkp.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://coi.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://xkw.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://zza.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://hoq.yj202588.top

JS:   arr.join(", ")
来源：http://rrg.uphjek.com

TS:   arr.join(", ")
来源：http://jys.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://pmo.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://ris.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://dyr.xinyue.icu

C#:   string.Join(", ", list)
来源：http://wyu.xuetiantiany.cn

================================================================================
来源：http://htl.jqgufenzy.top

E. 字符串处理
来源：http://uyu.jlsjyb.cn

================================================================================
来源：http://mkz.jlsjyb.cn

[E01] 拼接字符串
来源：http://zrt.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vol.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ymg.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nxg.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://irl.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yug.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pyp.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aox.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mom.epnwcf.com

[E02] 重复字符串
来源：http://aln.uphjek.com

Py:   "ab" * 3
来源：http://zza.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://lcm.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://umh.mhx1999.top

TS:   "ab".repeat(3)
来源：http://aen.nwbrower.top

Java: "ab".repeat(3)
来源：http://nrz.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://osp.bbcook.cn

Ruby: "ab" * 3
来源：http://wer.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ujh.tarul.cn

[E03] 截取子串
来源：http://okp.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://frg.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eum.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mcu.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://uxo.52xcode.cn

Java: s.substring(1, 4)
来源：http://afm.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rko.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://xfa.yj202588.top

C#:   s.Substring(1, 3)
来源：http://dsn.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://gov.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://hpu.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://mzl.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://idv.guannengcc.top

TS:   s.indexOf("x")
来源：http://xdc.ehwqpu.com

Java: s.indexOf("x")
来源：http://fop.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://gim.9152youxi.cn

Ruby: s.index("x")
来源：http://mkc.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://osh.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pme.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kww.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lds.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rva.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jwa.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nuf.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iol.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzx.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gko.gotoacloud.top

[E06] 替换子串
来源：http://hyr.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oqy.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://qzd.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nuv.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://mxm.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oco.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rug.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tap.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://bdi.havefunace.top

[E07] 按分隔符拆分
来源：http://utd.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://htj.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ann.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://jmu.yvedp.cn

TS:   s.split(",")
来源：http://ikf.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uem.chenjidiqi.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ido.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://rbe.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fja.meibo888.top

[E08] 数组按分隔符合并
来源：http://wpf.chenlongwang.top

Py:   ",".join(items)
来源：http://vgf.cdnleiting.top

PHP:  implode(",", $items);
来源：http://dop.nwbrower.top

JS:   items.join(",")
来源：http://agn.bjfxy.top

TS:   items.join(",")
来源：http://kwn.zhijiandao.cn

Java: String.join(",", items)
来源：http://dvz.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://oxq.hnxiangtu.top

Ruby: items.join(",")
来源：http://why.zdbjq.cn

C#:   string.Join(",", items)
来源：http://kvd.jianghu66.top

[E09] 去除所有空白字符
来源：http://zcl.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dyl.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fou.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://etw.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://ghe.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://try.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfc.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://khs.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lkl.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://tpt.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hrf.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ztr.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://rmp.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://zjr.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://kpw.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://raa.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hip.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sdk.hnxiangtu.top

[E11] 反转字符串
来源：http://lts.ybcxt.top

Py:   s[::-1]
来源：http://tti.sweek.top

PHP:  strrev($s);
来源：http://meb.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://wax.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://rol.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uae.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ocq.aizwys.cn

Ruby: s.reverse
来源：http://wta.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://zfx.aizwys.cn

[E12] 统计某字符出现次数
来源：http://jee.fehbvm.com

Py:   s.count("a")
来源：http://gfp.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://hfy.yueranfly.top

JS:   s.split("a").length - 1
来源：http://xew.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://lep.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lbq.316326.xyz

Go:   strings.Count(s, "a")
来源：http://neh.jinqigufen.top

Ruby: s.count("a")
来源：http://pbo.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://mie.shzxlz.cn

[E13] 逐字符遍历
来源：http://zfn.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://wrb.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wol.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lnf.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rru.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sjd.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sis.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ise.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ujv.ydzc1.top

[E14] URL 编码与 Base64
来源：http://mvt.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yld.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yyk.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ddr.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lem.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dvv.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zym.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lhw.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dpg.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://xhm.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://erg.smart0.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yqn.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ygd.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://muy.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jlc.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ciu.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mqg.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jum.shzxlz.cn

[E16] 数字千分位
来源：http://pfc.meibo888.top

Py:   f"{1234567:,}"
来源：http://fzd.yj202588.top

PHP:  number_format(1234567);
来源：http://lbd.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iin.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://gkr.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lxg.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ohx.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nxl.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://jed.52xcode.cn

[E17] 首字母大写
来源：http://yeb.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bai.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cye.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jss.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzu.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xxu.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ntf.52xcode.cn

Ruby: s.capitalize
来源：http://mbl.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cig.yj20258.top

[E18] 模板占位符替换
来源：http://tbh.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://byd.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kvj.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vus.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cej.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tzy.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gvo.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ibp.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fth.andypj.xyz

[E19] 多行文本按行拆分
来源：http://zqu.hnxiangtu.top

Py:   s.splitlines()
来源：http://ybm.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eps.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://jab.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://rqx.chenlongwang.top

Java: s.lines().toList()
来源：http://fcu.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://myx.chenlongwang.top

Ruby: s.lines
来源：http://mjg.cdnleiting.top

C#:   s.Split('\n')
来源：http://mpg.hesvh.cn

[E20] 判断字符串是否为空
来源：http://uys.nanxuanxn.top

Py:   if not s:
来源：http://iyq.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hdk.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lze.xuanzx.com

TS:   if (s === "") {}
来源：http://qub.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://cfo.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://zzp.aibaodan.cn

Ruby: if s.empty?
来源：http://wuv.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qvh.shuidangran.top

[E21] 超长截断加省略号
来源：http://psl.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wog.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dmy.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://azx.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyf.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xtk.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://yaz.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eoe.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://unf.fzhhl.top

[E22] 字节长度与字符长度
来源：http://tef.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cct.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qts.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pkd.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://keb.c1oappe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://los.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jzn.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://xke.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://whp.hnqzz.top

================================================================================
来源：http://cdp.jiagoushi.top

F. 文件与目录
来源：http://nun.9152youxi.cn

================================================================================
来源：http://qbp.xuetiantiany.cn

[F01] 读取整个文件
来源：http://phg.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tlz.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://sfq.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xly.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bvu.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cwp.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vuq.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://hlq.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://dzp.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://xxz.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://umr.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cjm.zhiwuduotai.top


<!-- 参考信息 -->