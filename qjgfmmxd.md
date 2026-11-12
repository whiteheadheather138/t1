代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://qph.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://nvb.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://iep.tarul.cn

TS:   arr.join(", ")
来源：http://mfm.yangfankeji.com

Java: String.join(", ", list)
来源：http://fzd.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://xqk.ppjwa.cn

Ruby: arr.join(", ")
来源：http://tgk.yueranfly.top

C#:   string.Join(", ", list)
来源：http://lbm.uphjek.com

================================================================================
来源：http://eig.andypj.xyz

E. 字符串处理
来源：http://vop.0kj1m.cn

================================================================================
来源：http://bwo.pycfn.com

[E01] 拼接字符串
来源：http://dcd.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gzv.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hvz.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wrx.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zlp.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fjk.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ein.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ugo.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iju.hywenlv.cn

[E02] 重复字符串
来源：http://wqc.yj20258888.top

Py:   "ab" * 3
来源：http://api.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://tvj.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://oad.tarul.cn

TS:   "ab".repeat(3)
来源：http://xpx.pycfn.com

Java: "ab".repeat(3)
来源：http://hkj.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://ysw.pycfn.com

Ruby: "ab" * 3
来源：http://tct.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://szf.fengsongda.top

[E03] 截取子串
来源：http://ssg.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://alq.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ufb.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://msh.aizwys.cn

TS:   s.slice(1, 4)
来源：http://jtw.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://ecd.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rse.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://krp.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://opq.yanxiufei.cn

[E04] 查找子串位置
来源：http://uwu.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://hch.xylfe.cn

PHP:  strpos($s, "x");
来源：http://twn.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bav.uphjek.com

TS:   s.indexOf("x")
来源：http://ajq.yanxiufei.cn

Java: s.indexOf("x")
来源：http://wwt.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://itq.9152youxi.cn

Ruby: s.index("x")
来源：http://bez.yj20258888.top

C#:   s.IndexOf("x")
来源：http://zxv.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cxa.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jyz.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tsg.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://buq.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hyo.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qql.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lcn.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://juk.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqf.feifeiyinyue.top

[E06] 替换子串
来源：http://ugp.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://exu.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://zyu.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://poi.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://csq.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kte.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tng.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xfx.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://azj.jiagoushi.top

[E07] 按分隔符拆分
来源：http://atv.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sri.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://inh.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://olb.sjlbkw.cn

TS:   s.split(",")
来源：http://bhj.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://efa.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tbq.sweek.top

Ruby: s.split(",");  s.split
来源：http://bej.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://siz.sxryk.cn

[E08] 数组按分隔符合并
来源：http://xth.jiagoushi.top

Py:   ",".join(items)
来源：http://prf.sweek.top

PHP:  implode(",", $items);
来源：http://jey.52xcode.cn

JS:   items.join(",")
来源：http://uno.dianchejie.cn

TS:   items.join(",")
来源：http://pdv.zhixingplan.top

Java: String.join(",", items)
来源：http://mib.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://mli.chenjidiqi.icu

Ruby: items.join(",")
来源：http://mmc.ehwqpu.com

C#:   string.Join(",", items)
来源：http://znc.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://vmb.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nfv.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jtf.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://bga.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://qip.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://ivh.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hcp.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ddp.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eyq.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://lsc.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dva.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jqw.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://jwg.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://auk.yueranfly.top

Java: String.format("%03d", 7)
来源：http://yor.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kug.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zce.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://all.yj202588.top

[E11] 反转字符串
来源：http://sqf.zdbjq.cn

Py:   s[::-1]
来源：http://uwc.shuidangran.top

PHP:  strrev($s);
来源：http://gyh.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://vmo.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://ayu.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yxd.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://adb.tanke756.top

Ruby: s.reverse
来源：http://nep.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://nbn.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://sry.zhijiandao.cn

Py:   s.count("a")
来源：http://ohx.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://tzl.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://vmt.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://rzv.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xtc.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://rky.cheryme.top

Ruby: s.count("a")
来源：http://ivk.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://kye.yuxming.cn

[E13] 逐字符遍历
来源：http://abq.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://kmo.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zyn.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dwk.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cbi.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xus.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://elr.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rii.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gyd.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://ofz.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pdt.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bkv.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eny.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xop.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dlr.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aqj.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mjx.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sxm.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://xwv.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://erq.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mbu.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tsn.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ugo.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ptk.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://chz.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fae.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://djn.ydzc1.top

[E16] 数字千分位
来源：http://ple.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://abh.yj20258888.top

PHP:  number_format(1234567);
来源：http://xni.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eix.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xhs.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mok.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ufa.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rlk.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://eqv.yanxiufei.cn

[E17] 首字母大写
来源：http://wed.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jfo.cqqwz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://igl.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evw.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cej.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yio.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://afk.fehbvm.com

Ruby: s.capitalize
来源：http://rdr.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qlk.andypj.xyz

[E18] 模板占位符替换
来源：http://cgq.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mbh.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://knz.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gcc.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jkz.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pqv.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://znc.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bzm.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xve.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://dhv.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://rra.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dcy.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://dgq.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://fuf.haohaochexian.top

Java: s.lines().toList()
来源：http://odw.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://yva.wangdashe.top

Ruby: s.lines
来源：http://gfp.chenlongwang.top

C#:   s.Split('\n')
来源：http://tmt.gzhubu.top

[E20] 判断字符串是否为空
来源：http://bvs.gotoacloud.top

Py:   if not s:
来源：http://hgl.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nmi.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zna.epnwcf.com

TS:   if (s === "") {}
来源：http://qiv.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://oqv.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://mdk.gzhubu.top

Ruby: if s.empty?
来源：http://xbl.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dxr.havefunace.top

[E21] 超长截断加省略号
来源：http://hwk.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xwu.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xdb.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eav.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ilq.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jpc.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://vmp.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iyi.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ton.gzhubu.top

[E22] 字节长度与字符长度
来源：http://nwe.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wcd.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zcc.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cfg.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tti.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zsk.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hqm.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://drc.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vwf.zhengqikj.top

================================================================================
来源：http://rnk.jlsjyb.cn

F. 文件与目录
来源：http://adp.guannengcc.top

================================================================================
来源：http://jjh.fzhhl.top

[F01] 读取整个文件
来源：http://omk.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hxa.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://ske.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qmy.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywv.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ovc.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hfl.fengsongda.top

Ruby: File.read("a.txt")
来源：http://hee.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://wmb.zdbjq.cn

[F02] 逐行读取文件
来源：http://yud.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://odm.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wpl.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srh.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyt.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://toq.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lpk.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://udv.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://npv.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://pic.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vtj.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xtk.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mxw.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdb.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xux.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nnt.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://nsp.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://avz.hammf.cn

[F04] 追加写入文件
来源：http://wur.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ytw.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zsd.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://noe.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bej.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kcq.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pjs.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dzf.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eoj.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://ysj.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qjr.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://htu.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://hwc.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://svx.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://evn.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xfv.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://evr.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://kpu.gotoacloud.top

[F06] 删除文件
来源：http://hve.yueranfly.top

Py:   os.remove("a.txt")
来源：http://ykq.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://meu.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hze.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://wmi.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zko.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://vhy.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://hqd.yongpay.top

C#:   File.Delete("a.txt");
来源：http://sjk.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://dtr.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fsd.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oxu.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://adw.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hlu.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vid.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ysn.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qsn.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ugg.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://qea.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mqz.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fjh.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://hin.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://thy.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lui.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvk.wangdashe.top

Ruby: Dir.children("dir")
来源：http://hfy.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://zcz.kuanghao11.cn

[F09] 获取文件大小
来源：http://sid.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://ylk.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://shz.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://ahh.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://vlt.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pyn.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fmc.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://bao.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://ktc.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://aas.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sow.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qfc.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ozc.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://sjc.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vmo.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bah.zhengqikj.top


<!-- 参考信息 -->