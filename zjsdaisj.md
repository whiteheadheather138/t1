代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hdb.xylfe.cn

JS:   arr.includes(x)
来源：http://kyg.ydzc1.top

TS:   arr.includes(x)
来源：http://dsf.nanxuanxn.top

Java: list.contains(x)
来源：http://wmh.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://zlr.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://gbb.wangdashe.top

C#:   list.Contains(x)
来源：http://fvf.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://mdc.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wuo.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://isp.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://irq.sysykeji.top

TS:   [...arr];
来源：http://jof.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://iqg.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://wil.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://xmm.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://vmq.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://mqs.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fwf.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oof.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qvr.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jsd.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gvj.vqdsnc.cn

Go:   // 手写循环
来源：http://jwq.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vbd.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kwo.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://ohv.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bvf.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pkr.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gls.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pnj.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xpu.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ycv.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sgp.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zka.yj20258.top

[D25] Set 集合去重与交并差
来源：http://crq.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jty.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jtq.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xyn.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fhw.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tqp.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://usq.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gle.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tef.hongshengwenyu.top

[D26] 数组转字符串
来源：http://mxn.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://wfq.tanke756.top

PHP:  implode(", ", $arr);
来源：http://ayo.iojbl.cn

JS:   arr.join(", ")
来源：http://szr.jqgfzy.top

TS:   arr.join(", ")
来源：http://rny.jqgufenzy.top

Java: String.join(", ", list)
来源：http://bys.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://rce.cashguo.top

Ruby: arr.join(", ")
来源：http://wxi.xinyue.icu

C#:   string.Join(", ", list)
来源：http://ccu.chenjidiqi.icu

================================================================================
来源：http://rxj.hnxiangtu.top

E. 字符串处理
来源：http://bfd.meibo888.top

================================================================================
来源：http://eul.hysaishi.cn

[E01] 拼接字符串
来源：http://awv.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xay.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jzf.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://obf.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lmx.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gei.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://crd.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jxa.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gmm.epnwcf.com

[E02] 重复字符串
来源：http://xpn.zhijiandao.cn

Py:   "ab" * 3
来源：http://kgu.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://fmc.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://krw.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://pdg.aizwys.cn

Java: "ab".repeat(3)
来源：http://xdm.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://fcj.ctjpmb.com

Ruby: "ab" * 3
来源：http://niv.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpb.guowangkeji.top

[E03] 截取子串
来源：http://mmw.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gli.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tkg.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zyg.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://pel.daxiang520.top

Java: s.substring(1, 4)
来源：http://vst.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://djr.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://pob.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://pol.zdqjudy.top

[E04] 查找子串位置
来源：http://uvd.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://krp.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://vcq.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pta.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://psc.aizwys.cn

Java: s.indexOf("x")
来源：http://uxy.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://knt.sweek.top

Ruby: s.index("x")
来源：http://qik.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://knk.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jiq.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dnh.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kwr.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpt.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://qsc.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dre.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://flu.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mlk.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oeu.shuidangran.top

[E06] 替换子串
来源：http://pqw.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wig.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://kdf.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pyc.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://wjf.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rum.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nva.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://daj.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://ssz.yuanzhike.top

[E07] 按分隔符拆分
来源：http://pai.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nyt.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hst.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jtk.jqgfzy.top

TS:   s.split(",")
来源：http://rik.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hcd.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tsf.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://nwg.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eez.yj20258.top

[E08] 数组按分隔符合并
来源：http://vbd.sysykeji.top

Py:   ",".join(items)
来源：http://fxo.gotoacloud.top

PHP:  implode(",", $items);
来源：http://qki.zdqjudy.top

JS:   items.join(",")
来源：http://ytp.fengsongda.top

TS:   items.join(",")
来源：http://hwa.jqgfzy.top

Java: String.join(",", items)
来源：http://gjc.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://pfq.xinyue.icu

Ruby: items.join(",")
来源：http://zbg.aibaodan.cn

C#:   string.Join(",", items)
来源：http://nlo.jqgfzy.top

[E09] 去除所有空白字符
来源：http://bhg.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eqo.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xox.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://xcy.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://jiu.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://svg.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oxe.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qqh.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sak.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://jhx.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oct.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hul.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://uvd.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://tob.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://qbv.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mke.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ydk.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mxm.redwolf501.top

[E11] 反转字符串
来源：http://yyr.yuanzhike.top

Py:   s[::-1]
来源：http://mae.meibo888.top

PHP:  strrev($s);
来源：http://mbh.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://umf.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://syk.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://idx.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vmy.ppjwa.cn

Ruby: s.reverse
来源：http://nnu.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://kiv.sweek.top

[E12] 统计某字符出现次数
来源：http://xlm.zycfv.cn

Py:   s.count("a")
来源：http://ous.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://iai.cashguo.top

JS:   s.split("a").length - 1
来源：http://iyo.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://zmx.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ffe.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://tcd.cucudq.cn

Ruby: s.count("a")
来源：http://tfc.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://rni.xuanzx.com

[E13] 逐字符遍历
来源：http://ngq.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://vlu.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wug.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://itl.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vbw.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hyj.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rsh.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rwt.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eod.c1oappe.top

[E14] URL 编码与 Base64
来源：http://lgs.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zkl.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xsv.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baf.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tdr.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lrk.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pwx.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tyu.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lna.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://izg.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wkk.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vsa.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fvd.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hpk.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://utq.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tvi.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://prb.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sxp.shzxlz.cn

[E16] 数字千分位
来源：http://gej.xinyue.icu

Py:   f"{1234567:,}"
来源：http://wpe.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://nmg.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tvb.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rjw.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hmw.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bbd.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pxu.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://tdj.hnxiangtu.top

[E17] 首字母大写
来源：http://xzg.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dwu.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jrr.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aut.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajc.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kdd.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pso.hnqzz.top

Ruby: s.capitalize
来源：http://hbd.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xpm.yangfankeji.com

[E18] 模板占位符替换
来源：http://fft.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ipi.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://moe.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yxz.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ilr.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmo.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rgi.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dio.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cya.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://riw.yj202588.top

Py:   s.splitlines()
来源：http://hks.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wbn.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://fbm.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://zut.snrcjt.cn

Java: s.lines().toList()
来源：http://sik.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://uts.ehwqpu.com

Ruby: s.lines
来源：http://rfx.quarkkingdee.top

C#:   s.Split('\n')
来源：http://eii.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://hzk.pycfn.com

Py:   if not s:
来源：http://cxt.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nng.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kta.chenlongwang.top

TS:   if (s === "") {}
来源：http://eqx.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://trs.nwbrower.top

Go:   if s == "" {}
来源：http://zyf.dianchejie.cn

Ruby: if s.empty?
来源：http://cic.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xtm.bjfxy.top

[E21] 超长截断加省略号
来源：http://uzz.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jkk.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ejr.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bed.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qak.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qzx.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://hoc.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zyc.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tws.pycfn.com

[E22] 字节长度与字符长度
来源：http://kci.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txq.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://orf.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcj.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mnx.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uej.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tsq.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://icx.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aqh.zycfv.cn

================================================================================
来源：http://jnj.ywan-chungtsiang.top

F. 文件与目录
来源：http://jka.shanyushiyangtech.top

================================================================================
来源：http://chs.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://sft.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jsp.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://ldj.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zfw.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bte.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vhi.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eeg.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://oaj.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://oqe.zdqjudy.top

[F02] 逐行读取文件
来源：http://hpk.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mdp.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nxk.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ovx.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xoz.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://skj.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pnb.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gih.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rse.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://des.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://izx.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zlo.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kog.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vra.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ohl.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://suy.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://nal.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eei.zycfv.cn

[F04] 追加写入文件
来源：http://pec.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jis.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zfk.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rdu.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbr.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dkc.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nlg.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mfe.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xbg.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://xbo.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qhc.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://vkm.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://gwk.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://kcm.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bzc.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dhd.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://pqa.tarul.cn


<!-- 参考信息 -->