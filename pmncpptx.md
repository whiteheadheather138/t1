代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://giw.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://jxo.fengsongda.top

Py:   Counter(arr)
来源：http://ydp.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://xmx.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hup.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uol.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lij.mhx1999.top

Go:   // 手写 map[T]int
来源：http://sae.cdnleiting.top

Ruby: arr.tally
来源：http://nyb.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nyx.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://voe.yvedp.cn

Py:   x in arr
来源：http://pjf.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://tqu.uphjek.com

JS:   arr.includes(x)
来源：http://bvm.0kj1m.cn

TS:   arr.includes(x)
来源：http://fmw.yangfankeji.com

Java: list.contains(x)
来源：http://sru.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://rbw.birdmap.top

Ruby: arr.include?(x)
来源：http://hce.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://jlz.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://bmp.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sdd.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gkn.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kpt.yj20258.top

TS:   [...arr];
来源：http://gjj.fengsongda.top

Java: new ArrayList<>(list);
来源：http://hlf.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vdq.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://oms.0kj1m.cn

C#:   new List<int>(list);
来源：http://efd.hnxiangtu.top

[D23] reduce 累积计算
来源：http://sgp.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vwi.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ygi.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znd.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qso.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cxb.aizwys.cn

Go:   // 手写循环
来源：http://skx.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bbf.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gyi.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://tgl.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ror.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cjc.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbx.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://czg.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://roe.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yde.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bbm.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jag.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://mhl.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hbe.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mhm.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kgt.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zkv.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oux.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rrc.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://spq.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qnj.epnwcf.com

[D26] 数组转字符串
来源：http://rfe.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://yst.316326.xyz

PHP:  implode(", ", $arr);
来源：http://ivm.hywenlv.cn

JS:   arr.join(", ")
来源：http://sdr.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://iqb.sweek.top

Java: String.join(", ", list)
来源：http://iwf.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://wxg.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://dkx.hesvh.cn

C#:   string.Join(", ", list)
来源：http://qgt.tanke756.top

================================================================================
来源：http://zmw.sweek.top

E. 字符串处理
来源：http://syt.hywenlv.cn

================================================================================
来源：http://biu.daria6918.cn

[E01] 拼接字符串
来源：http://znu.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uty.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sdi.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbc.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nfj.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fmb.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tis.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nbe.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://acx.hammf.cn

[E02] 重复字符串
来源：http://uic.bbcook.cn

Py:   "ab" * 3
来源：http://ofo.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://hnr.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://sdh.yj20258.top

TS:   "ab".repeat(3)
来源：http://bki.0kj1m.cn

Java: "ab".repeat(3)
来源：http://tbt.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://tsg.snrcjt.cn

Ruby: "ab" * 3
来源：http://phh.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://flr.jinqigufen.top

[E03] 截取子串
来源：http://dib.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ptt.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fxh.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jyj.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://jda.cucudq.cn

Java: s.substring(1, 4)
来源：http://jve.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eov.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lmd.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://lbh.pycfn.com

[E04] 查找子串位置
来源：http://vwj.nanxinkj.top

Py:   s.find("x");  s.index("x")
来源：http://jbm.hcnkem.com

PHP:  strpos($s, "x");
来源：http://aln.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nsi.jinqigufen.top

TS:   s.indexOf("x")
来源：http://xju.mhx1999.top

Java: s.indexOf("x")
来源：http://brc.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://kwi.fengsongda.top

Ruby: s.index("x")
来源：http://ikd.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://vvp.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vxj.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dae.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pfx.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qnz.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dmu.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzv.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aji.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pcg.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rvn.hammf.cn

[E06] 替换子串
来源：http://bsu.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jmz.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ttl.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hue.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://txv.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mqb.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ueo.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vmu.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://ztv.jiagoushi.top

[E07] 按分隔符拆分
来源：http://eon.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mqj.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mcd.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://epo.tian-w.cn

TS:   s.split(",")
来源：http://num.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://msy.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://znx.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://hzi.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fng.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://yzn.kuanghao11.cn

Py:   ",".join(items)
来源：http://smk.pycfn.com

PHP:  implode(",", $items);
来源：http://hje.gzhubu.top

JS:   items.join(",")
来源：http://rrw.xuanzx.com

TS:   items.join(",")
来源：http://rpi.guannengcc.top

Java: String.join(",", items)
来源：http://yvv.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://ked.aibaodan.cn

Ruby: items.join(",")
来源：http://eye.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://jis.sysykeji.top

[E09] 去除所有空白字符
来源：http://hzp.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nxb.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcx.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://vxl.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://lfv.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://irq.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://rne.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://dhd.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ulq.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://lch.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://snj.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xch.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://kuh.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://ywm.hcnkem.com

Java: String.format("%03d", 7)
来源：http://owy.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vvg.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dvs.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sap.yonumen.top

[E11] 反转字符串
来源：http://tul.fehbvm.com

Py:   s[::-1]
来源：http://azm.zdbjq.cn

PHP:  strrev($s);
来源：http://cgm.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://krm.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://wxq.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hsc.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lyu.jianghu66.top

Ruby: s.reverse
来源：http://hfj.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://sxt.shuidangran.top

[E12] 统计某字符出现次数
来源：http://clr.fanxiaobao.xyz

Py:   s.count("a")
来源：http://xkl.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://zzi.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://wsq.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://vmz.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gww.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://whf.nwbrower.top

Ruby: s.count("a")
来源：http://rtf.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://yzr.tianlin.xyz

[E13] 逐字符遍历
来源：http://lmg.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://yav.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fva.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ccm.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://smu.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qzx.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qfy.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vpn.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://abe.yuxming.cn

[E14] URL 编码与 Base64
来源：http://xcf.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vey.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xbi.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fke.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://coc.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kaq.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sgg.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pww.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wkm.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://pio.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ess.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blz.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cco.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://puv.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vgi.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rbl.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fsk.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://civ.zycfv.cn

[E16] 数字千分位
来源：http://ebh.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://swb.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://pqi.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://pwg.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zbt.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ksi.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hiv.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lqc.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://olt.ppjwa.cn

[E17] 首字母大写
来源：http://lad.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://knx.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hrt.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wfl.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ioe.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iws.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wkm.vqdsnc.cn

Ruby: s.capitalize
来源：http://zjt.uphjek.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ezb.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://ykq.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://msx.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uau.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lgi.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gib.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mto.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xkv.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://faw.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://udr.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://nmu.havefunace.top

Py:   s.splitlines()
来源：http://dfe.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dgs.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://hij.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://ftb.sxryk.cn

Java: s.lines().toList()
来源：http://nnj.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://gqc.xuetiantiany.cn

Ruby: s.lines
来源：http://xik.tianlin.xyz

C#:   s.Split('\n')
来源：http://qph.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://rhd.fehbvm.com

Py:   if not s:
来源：http://cyk.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jqh.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hdg.shzxlz.cn

TS:   if (s === "") {}
来源：http://sok.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://uzs.ivvv.top

Go:   if s == "" {}
来源：http://vrt.gaohongyu789.top

Ruby: if s.empty?
来源：http://eyo.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://icj.yangfankeji.com

[E21] 超长截断加省略号
来源：http://vqt.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://krn.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vvc.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwx.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pmt.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://smb.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://yjt.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://npx.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://klx.yuxming.cn

[E22] 字节长度与字符长度
来源：http://nou.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vpr.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://njl.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://grh.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ozq.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://omg.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jgd.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://jgu.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xfi.shangyingyoupin.top

================================================================================
来源：http://mox.yj20258888.top

F. 文件与目录
来源：http://kus.gaohongyu789.top

================================================================================
来源：http://ohl.ehwqpu.com

[F01] 读取整个文件
来源：http://xuw.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://syn.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://xhj.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ino.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rmg.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bkx.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ysg.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://rwo.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://hgz.dianchejie.cn

[F02] 逐行读取文件
来源：http://rdc.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hrf.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bqp.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uog.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcv.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xvq.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ujm.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jbo.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oqa.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://qwl.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fnz.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mfc.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dza.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hoe.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://znj.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tfv.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://nsb.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cmq.nwbrower.top

[F04] 追加写入文件
来源：http://bis.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sjs.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wqx.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebs.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qah.kuanghao11.cn


<!-- 参考信息 -->