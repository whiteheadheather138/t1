代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://npl.meibo888.top

[D20] 统计每个元素出现次数
来源：http://jio.hammf.cn

Py:   Counter(arr)
来源：http://tai.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://gbk.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oij.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vmd.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xuj.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://lpj.shzxlz.cn

Ruby: arr.tally
来源：http://iwr.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dtw.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://zir.yfazqb.com

Py:   x in arr
来源：http://des.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://ebi.0kj1m.cn

JS:   arr.includes(x)
来源：http://aac.hnxiangtu.top

TS:   arr.includes(x)
来源：http://cer.epnwcf.com

Java: list.contains(x)
来源：http://bxi.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://tha.dashuyun.cn

Ruby: arr.include?(x)
来源：http://jsq.yj202588.top

C#:   list.Contains(x)
来源：http://opv.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://blf.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ovt.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://prv.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qtb.cucudq.cn

TS:   [...arr];
来源：http://hkb.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://pqt.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://gcn.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://tfa.zhijiandao.cn

C#:   new List<int>(list);
来源：http://gwt.snrcjt.cn

[D23] reduce 累积计算
来源：http://yam.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://crn.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qyn.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eag.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ubh.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ipm.fzhhl.top

Go:   // 手写循环
来源：http://syx.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nqn.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zgt.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://wag.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nwm.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rgu.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bhi.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wqd.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://boh.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewy.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tmg.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hoe.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://gpl.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tzc.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://twy.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ier.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ezi.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zjk.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vam.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://myh.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wdt.hysaishi.cn

[D26] 数组转字符串
来源：http://umr.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://avg.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://bdx.yonumen.top

JS:   arr.join(", ")
来源：http://nsw.ctjpmb.com

TS:   arr.join(", ")
来源：http://xzk.yongpay.top

Java: String.join(", ", list)
来源：http://rwk.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://rtf.jinqigufen.top

Ruby: arr.join(", ")
来源：http://xtv.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://lnr.hcnkem.com

================================================================================
来源：http://xyq.andypj.xyz

E. 字符串处理
来源：http://rxo.jqgufenzy.top

================================================================================
来源：http://hwk.yonumen.top

[E01] 拼接字符串
来源：http://kgj.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cio.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fjl.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pqj.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zwt.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nen.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mxh.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cet.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uox.tanke756.top

[E02] 重复字符串
来源：http://qem.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://zca.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://jfu.hnqzz.top

JS:   "ab".repeat(3)
来源：http://cyl.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://ddp.meibo888.top

Java: "ab".repeat(3)
来源：http://mmb.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://hnn.chenlongwang.top

Ruby: "ab" * 3
来源：http://uqi.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://liv.ppjwa.cn

[E03] 截取子串
来源：http://kyt.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oln.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zzf.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qlt.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://irg.jianghu66.top

Java: s.substring(1, 4)
来源：http://ocq.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tpl.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://qst.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://lyu.birdmap.top

[E04] 查找子串位置
来源：http://nxd.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://wqh.mhx1999.top

PHP:  strpos($s, "x");
来源：http://ylr.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xfv.0kj1m.cn

TS:   s.indexOf("x")
来源：http://zdt.bjfxy.top

Java: s.indexOf("x")
来源：http://alq.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://vgk.hysaishi.cn

Ruby: s.index("x")
来源：http://ivg.yueranfly.top

C#:   s.IndexOf("x")
来源：http://hok.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xwc.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://beu.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hpp.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jay.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tip.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvq.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mlu.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hda.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://brr.havefunace.top

[E06] 替换子串
来源：http://axn.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://psi.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://kog.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mps.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://ifv.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yee.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tys.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gtp.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://afw.havefunace.top

[E07] 按分隔符拆分
来源：http://qrb.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nau.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bnl.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jna.epnwcf.com

TS:   s.split(",")
来源：http://nno.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://pvm.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nfd.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://yrp.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bez.c1oappe.top

[E08] 数组按分隔符合并
来源：http://jpz.hcnkem.com

Py:   ",".join(items)
来源：http://dyd.52xcode.cn

PHP:  implode(",", $items);
来源：http://day.birdmap.top

JS:   items.join(",")
来源：http://njz.hysaishi.cn

TS:   items.join(",")
来源：http://tit.bbcook.cn

Java: String.join(",", items)
来源：http://ruu.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://xvg.fehbvm.com

Ruby: items.join(",")
来源：http://lln.smart0.xyz

C#:   string.Join(",", items)
来源：http://lwu.yuxming.cn

[E09] 去除所有空白字符
来源：http://hjd.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gyi.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pii.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://wqi.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://bjl.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ojn.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ybv.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fjy.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gso.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://pgz.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cna.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cky.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://vdc.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://urm.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://nyt.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qxs.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://odt.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ids.yuxming.cn

[E11] 反转字符串
来源：http://xit.0kj1m.cn

Py:   s[::-1]
来源：http://uia.zycfv.cn

PHP:  strrev($s);
来源：http://uug.yongpay.top

JS:   [...s].reverse().join("")
来源：http://nno.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://qol.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://deg.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yta.tianlin.xyz

Ruby: s.reverse
来源：http://agq.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lmy.sweek.top

[E12] 统计某字符出现次数
来源：http://ttx.hammf.cn

Py:   s.count("a")
来源：http://eep.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://usk.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://hlb.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://acg.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fvp.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://cgp.hnxiangtu.top

Ruby: s.count("a")
来源：http://oeu.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://goi.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://rlj.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://cin.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jdm.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://lqm.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vow.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oyj.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dsi.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zdr.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lej.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://dxz.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://elp.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vze.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jwr.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zqw.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ouy.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ovt.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tuh.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eze.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://abu.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qlb.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rll.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tvz.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vlx.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ijb.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://arj.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zdu.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yxv.ppjwa.cn

[E16] 数字千分位
来源：http://hkt.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://hkb.aizwys.cn

PHP:  number_format(1234567);
来源：http://iuw.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://pjy.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pvh.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mre.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jgb.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lxg.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://vtd.hammf.cn

[E17] 首字母大写
来源：http://avs.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gve.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cwi.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsw.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yxv.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yke.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vsp.yonumen.top

Ruby: s.capitalize
来源：http://gzm.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uwd.hfpthk.cn

[E18] 模板占位符替换
来源：http://poa.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kcv.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cfi.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rpa.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fri.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://spv.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dos.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xad.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://plm.9152youxi.cn

[E19] 多行文本按行拆分
来源：http://uzo.wangdashe.top

Py:   s.splitlines()
来源：http://nik.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://imo.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://nry.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://ieb.tianlin.xyz

Java: s.lines().toList()
来源：http://kyy.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://sek.zdbjq.cn

Ruby: s.lines
来源：http://iqv.mhx1999.top

C#:   s.Split('\n')
来源：http://qov.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://cxo.316326.xyz

Py:   if not s:
来源：http://atg.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://npf.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://chu.xylfe.cn

TS:   if (s === "") {}
来源：http://bja.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://ile.svipenyu.cn

Go:   if s == "" {}
来源：http://atp.mhx1999.top

Ruby: if s.empty?
来源：http://ghr.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fjw.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://yhz.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dmx.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lok.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://miv.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dev.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xlf.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://kyq.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jgn.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://egj.daxiang520.top

[E22] 字节长度与字符长度
来源：http://iaf.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qwm.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://upy.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aby.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjd.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zci.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nqh.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://tgh.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bny.mhx1999.top

================================================================================
来源：http://qnc.yongpay.top

F. 文件与目录
来源：http://ffa.aibaodan.cn

================================================================================
来源：http://dru.hysaishi.cn

[F01] 读取整个文件
来源：http://zfa.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://txd.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://wez.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vyx.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xgk.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qcj.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fpu.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://xjh.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://uak.meibo888.top

[F02] 逐行读取文件
来源：http://rxc.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nyo.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dzg.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzs.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gyj.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://drm.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fuc.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oui.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://thp.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://owl.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgz.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vgs.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ncn.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://khi.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wgh.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qqf.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://afu.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qnv.yangfankeji.com

[F04] 追加写入文件
来源：http://qpf.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hdw.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tgx.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxr.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oon.feifeiyinyue.top


<!-- 参考信息 -->