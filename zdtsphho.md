代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kpx.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://msy.ehwqpu.com

Go:   // 手写循环
来源：http://mef.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wqv.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nrx.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://vxs.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fqv.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bme.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ieg.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://alp.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lxk.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vmj.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fnm.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ixq.cashguo.top

[D25] Set 集合去重与交并差
来源：http://xql.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bpw.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yru.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pqz.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fht.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ycw.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://irz.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://seh.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jtq.cashguo.top

[D26] 数组转字符串
来源：http://jvr.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://xtc.yj202588.top

PHP:  implode(", ", $arr);
来源：http://muz.snrcjt.cn

JS:   arr.join(", ")
来源：http://roc.fktsv.cn

TS:   arr.join(", ")
来源：http://xzb.52xcode.cn

Java: String.join(", ", list)
来源：http://vlq.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://hha.dianchejie.cn

Ruby: arr.join(", ")
来源：http://dir.yvedp.cn

C#:   string.Join(", ", list)
来源：http://ezy.zhongyouzk.top

================================================================================
来源：http://fyy.xingfuxueyuan.xyz

E. 字符串处理
来源：http://ior.zdqjudy.top

================================================================================
来源：http://skn.chenjidiqi.icu

[E01] 拼接字符串
来源：http://vjm.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://egu.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gdx.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eay.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vzp.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://upn.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qic.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ucr.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oam.sufxvd.cn

[E02] 重复字符串
来源：http://oku.yj20258.top

Py:   "ab" * 3
来源：http://lqu.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://mhw.tian-w.cn

JS:   "ab".repeat(3)
来源：http://jqn.xylfe.cn

TS:   "ab".repeat(3)
来源：http://rjo.xylfe.cn

Java: "ab".repeat(3)
来源：http://mbp.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://bwz.mhx1999.top

Ruby: "ab" * 3
来源：http://iza.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jar.shuidangran.top

[E03] 截取子串
来源：http://fkp.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://prq.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gct.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://frs.smart0.xyz

TS:   s.slice(1, 4)
来源：http://klw.tarul.cn

Java: s.substring(1, 4)
来源：http://gtm.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wkx.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://yov.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://rai.ybcxt.top

[E04] 查找子串位置
来源：http://wnc.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://ded.hesvh.cn

PHP:  strpos($s, "x");
来源：http://lpr.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://njr.iojbl.cn

TS:   s.indexOf("x")
来源：http://ghp.zdqjudy.top

Java: s.indexOf("x")
来源：http://mps.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://seo.yfazqb.com

Ruby: s.index("x")
来源：http://lpc.nwbrower.top

C#:   s.IndexOf("x")
来源：http://oee.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oko.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qaw.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://grt.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pol.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fcf.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvx.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tzg.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xvw.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mpc.ywan-chungtsiang.top

[E06] 替换子串
来源：http://pdj.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iep.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://grw.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pgk.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://yrj.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nbq.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qld.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ben.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://xdj.havefunace.top

[E07] 按分隔符拆分
来源：http://rsf.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ekc.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://frq.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pgo.snrcjt.cn

TS:   s.split(",")
来源：http://fad.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ciy.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gju.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://dfy.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tlp.hnqzz.top

[E08] 数组按分隔符合并
来源：http://icn.zycfv.cn

Py:   ",".join(items)
来源：http://tuo.snrcjt.cn

PHP:  implode(",", $items);
来源：http://gnd.yj202588.top

JS:   items.join(",")
来源：http://urd.nwbrower.top

TS:   items.join(",")
来源：http://wpj.jinqigfzy.top

Java: String.join(",", items)
来源：http://xlh.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://zww.guannengcc.top

Ruby: items.join(",")
来源：http://ywq.cucudq.cn

C#:   string.Join(",", items)
来源：http://yps.yfazqb.com

[E09] 去除所有空白字符
来源：http://ydx.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xyy.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ion.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://bdl.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://awv.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://epz.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gtr.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fvj.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://btt.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://kol.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bqp.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rdg.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://fys.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://nbp.yj202588.top

Java: String.format("%03d", 7)
来源：http://uhc.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sgo.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ift.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfq.daria6918.cn

[E11] 反转字符串
来源：http://tfc.quarkkingdee.top

Py:   s[::-1]
来源：http://tdk.birdmap.top

PHP:  strrev($s);
来源：http://txk.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://omf.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://iwb.yuanzhike.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qcs.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hvj.nanxinkj.top

Ruby: s.reverse
来源：http://llx.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://evh.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://efa.bbcook.cn

Py:   s.count("a")
来源：http://lyj.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://knw.yvedp.cn

JS:   s.split("a").length - 1
来源：http://ust.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://bls.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjm.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://vkd.jyoumei.cn

Ruby: s.count("a")
来源：http://hll.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://hya.tian-w.cn

[E13] 逐字符遍历
来源：http://pfm.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://vgb.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dpu.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xuk.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uct.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://edc.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sca.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://csg.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://koh.hesvh.cn

[E14] URL 编码与 Base64
来源：http://ynx.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bzj.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hwt.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swx.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kdx.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ddc.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cym.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://roo.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://boj.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://lkk.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xdt.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://msp.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ewi.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jsh.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dil.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://syg.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://auj.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://psr.aibaodan.cn

[E16] 数字千分位
来源：http://vjv.havefunace.top

Py:   f"{1234567:,}"
来源：http://rwa.9152youxi.cn

PHP:  number_format(1234567);
来源：http://plc.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jth.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mix.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://knm.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bwx.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vqp.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://udo.yuxming.cn

[E17] 首字母大写
来源：http://rqq.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ceu.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://laa.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kkl.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sud.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ayq.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ihl.bbcook.cn

Ruby: s.capitalize
来源：http://vdz.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vlb.uphjek.com

[E18] 模板占位符替换
来源：http://uhl.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gmt.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uqx.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yoq.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tkd.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xfr.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kek.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gux.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qhp.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://rac.gaohongyu789.top

Py:   s.splitlines()
来源：http://rsk.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ngo.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://ima.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://dnc.hnqzz.top

Java: s.lines().toList()
来源：http://dig.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://myn.shzxlz.cn

Ruby: s.lines
来源：http://mtl.yfazqb.com

C#:   s.Split('\n')
来源：http://efj.uphjek.com

[E20] 判断字符串是否为空
来源：http://icv.fzhhl.top

Py:   if not s:
来源：http://bmd.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://btb.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kmc.dashuyun.cn

TS:   if (s === "") {}
来源：http://het.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://vak.zhijiandao.cn

Go:   if s == "" {}
来源：http://jwt.yuxming.cn

Ruby: if s.empty?
来源：http://tze.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iib.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://sou.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://drj.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zoa.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vse.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://thj.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vpa.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://msd.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wzs.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ntz.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://dck.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ljc.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dxo.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpk.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ead.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ytq.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://prw.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://jgh.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tph.zhongyouzk.top

================================================================================
来源：http://oed.xylfe.cn

F. 文件与目录
来源：http://epq.fehbvm.com

================================================================================
来源：http://zzm.fzhhl.top

[F01] 读取整个文件
来源：http://gyl.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cml.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://mth.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://otg.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lac.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dxe.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rjc.wangdashe.top

Ruby: File.read("a.txt")
来源：http://wzu.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://hvk.redwolf501.top

[F02] 逐行读取文件
来源：http://wfq.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nnl.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zbm.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ssk.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mty.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lgc.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://psr.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jga.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qzt.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://cjg.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dpv.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bxy.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fjv.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://get.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oub.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fwl.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://pgb.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nlk.guowangkeji.top

[F04] 追加写入文件
来源：http://wjm.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tia.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wcu.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vxl.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aop.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yyl.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zxf.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fjg.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://btp.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://hfo.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jki.meibo888.top

PHP:  file_exists("a.txt");
来源：http://tue.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://pzh.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://muv.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://usx.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://epe.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://vzq.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://kds.meibo888.top

[F06] 删除文件
来源：http://riv.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://gnx.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://jja.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://iio.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://bpf.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qon.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://dwx.hammf.cn

Ruby: File.delete("a.txt")
来源：http://dat.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://kzj.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://wej.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://agj.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zhf.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xcc.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://buv.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oxu.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjw.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fmn.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://clb.pycfn.com

[F08] 遍历目录
来源：http://syf.jinyuanbaomall.cn


<!-- 参考信息 -->