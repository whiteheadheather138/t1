代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hak.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jtg.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kbt.yuanzhike.top

[D26] 数组转字符串
来源：http://wpr.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://gvy.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://ets.sxryk.cn

JS:   arr.join(", ")
来源：http://uas.vqdsnc.cn

TS:   arr.join(", ")
来源：http://rpq.svipenyu.cn

Java: String.join(", ", list)
来源：http://xrn.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://pgv.cdnleiting.top

Ruby: arr.join(", ")
来源：http://jzo.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://tru.gaohongyu789.top

================================================================================
来源：http://qgc.yj20258.top

E. 字符串处理
来源：http://unr.ydzc1.top

================================================================================
来源：http://dyo.jyoumei.cn

[E01] 拼接字符串
来源：http://tyu.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gyo.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://won.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofd.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eeb.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ihj.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hxz.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cks.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qzq.birdmap.top

[E02] 重复字符串
来源：http://dwf.epnwcf.com

Py:   "ab" * 3
来源：http://nfb.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://muh.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://smc.jianghu66.top

TS:   "ab".repeat(3)
来源：http://fny.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://zel.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://agt.fktsv.cn

Ruby: "ab" * 3
来源：http://skd.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eex.guannengcc.top

[E03] 截取子串
来源：http://ifz.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://odn.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://icg.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zoz.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://ehq.yj202588.top

Java: s.substring(1, 4)
来源：http://jdp.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://plt.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://kvj.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://vba.zhiwuduotai.top

[E04] 查找子串位置
来源：http://bfj.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://lbd.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://gui.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xqn.ppjwa.cn

TS:   s.indexOf("x")
来源：http://pos.c1oappe.top

Java: s.indexOf("x")
来源：http://mws.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://rzo.yvedp.cn

Ruby: s.index("x")
来源：http://ypi.52xcode.cn

C#:   s.IndexOf("x")
来源：http://pse.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ywe.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://djl.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uxf.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwo.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://mnc.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yph.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ujo.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qox.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wxr.sweek.top

[E06] 替换子串
来源：http://fjh.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vgo.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://yax.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jgc.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://cox.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jqr.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ksa.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gcv.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://mzz.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://btx.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://boa.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qtc.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://vyi.shangyingyoupin.top

TS:   s.split(",")
来源：http://mfe.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://bvm.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bcx.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://aez.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rnl.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://ssq.snrcjt.cn

Py:   ",".join(items)
来源：http://mun.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://gzk.nwbrower.top

JS:   items.join(",")
来源：http://hwt.sysykeji.top

TS:   items.join(",")
来源：http://eel.yangfankeji.com

Java: String.join(",", items)
来源：http://por.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://kzr.yfazqb.com

Ruby: items.join(",")
来源：http://rwd.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://vyi.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://rvz.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jpz.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xim.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://rzi.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://obf.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://lxh.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vfk.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zuv.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://efh.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://wcl.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://swq.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hcx.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://muj.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://xcs.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://aud.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wdm.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tgf.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tqz.yuxming.cn

[E11] 反转字符串
来源：http://xcd.zhiwuduotai.top

Py:   s[::-1]
来源：http://usv.svipenyu.cn

PHP:  strrev($s);
来源：http://rmq.havefunace.top

JS:   [...s].reverse().join("")
来源：http://eoe.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://wco.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jhk.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dnu.jyoumei.cn

Ruby: s.reverse
来源：http://sgv.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://jbi.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://qgf.zhoulong.xyz

Py:   s.count("a")
来源：http://eol.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://hvt.c1oappe.top

JS:   s.split("a").length - 1
来源：http://oub.daxiang520.top

TS:   s.split("a").length - 1
来源：http://drb.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mng.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://dgj.nanxinkj.top

Ruby: s.count("a")
来源：http://jhp.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://kfj.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://vhb.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://vra.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xnl.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lkj.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zad.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wbk.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mrt.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gcu.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://klm.iojbl.cn

[E14] URL 编码与 Base64
来源：http://syf.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xed.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zrx.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lve.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rph.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zit.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vom.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ttq.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://psb.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://thp.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xes.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://irq.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dwv.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gka.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://slj.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ojx.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://efw.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cul.daria6918.cn

[E16] 数字千分位
来源：http://xou.zycfv.cn

Py:   f"{1234567:,}"
来源：http://tst.yuanzhike.top

PHP:  number_format(1234567);
来源：http://wpz.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uhr.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wfw.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://utg.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://omh.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cxc.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://gyb.sufxvd.cn

[E17] 首字母大写
来源：http://lwb.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aqw.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihi.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nwz.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wqd.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sat.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ayr.zdqjudy.top

Ruby: s.capitalize
来源：http://mol.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://edn.ivvv.top

[E18] 模板占位符替换
来源：http://tyy.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cxg.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fdu.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://flo.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cex.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rtx.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bzq.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fjr.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wdc.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://emh.yuxming.cn

Py:   s.splitlines()
来源：http://xfa.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tig.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://yku.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://kky.hywenlv.cn

Java: s.lines().toList()
来源：http://zcj.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://ian.chenzaomai.com

Ruby: s.lines
来源：http://vyr.fengsongda.top

C#:   s.Split('\n')
来源：http://pwx.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://eci.daxiang520.top

Py:   if not s:
来源：http://buj.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cdx.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fcn.zhongyouzk.top

TS:   if (s === "") {}
来源：http://jmc.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://hlf.smart0.xyz

Go:   if s == "" {}
来源：http://auj.yonumen.top

Ruby: if s.empty?
来源：http://uph.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://daf.fehbvm.com

[E21] 超长截断加省略号
来源：http://qhr.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xxl.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wkt.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rzu.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yby.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mde.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://jqc.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zso.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ibh.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://huc.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dak.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ubl.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wzg.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ygv.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yra.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iui.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://cvz.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bjt.hywenlv.cn

================================================================================
来源：http://fhc.0kj1m.cn

F. 文件与目录
来源：http://qjl.nanxinkj.top

================================================================================
来源：http://mrm.gotoacloud.top

[F01] 读取整个文件
来源：http://zvy.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eku.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://omo.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rwp.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xmk.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vlr.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://chx.cheryme.top

Ruby: File.read("a.txt")
来源：http://ohj.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://izm.tarul.cn

[F02] 逐行读取文件
来源：http://mbw.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qpr.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://des.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwi.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swk.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ctc.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ngs.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uvt.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gbl.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://jks.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qye.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jst.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xgx.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwr.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nzy.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uil.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://fox.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dbk.ppjwa.cn

[F04] 追加写入文件
来源：http://wjn.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ijt.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mqn.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lre.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vgn.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ele.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bwm.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qdz.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://drc.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://nxf.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fia.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://mow.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://jvn.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://orx.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wxf.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jtp.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://rst.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://llr.yj20258.top

[F06] 删除文件
来源：http://vqs.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://jgn.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://vek.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://zhl.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gbh.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bbs.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://crd.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://kbn.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://ybf.52xcode.cn

[F07] 创建目录（含多级）
来源：http://amq.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eij.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lcv.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndv.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hor.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dxv.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://odi.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ajg.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hvm.316326.xyz

[F08] 遍历目录
来源：http://kaa.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://phx.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gvl.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://qvw.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://iky.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ymc.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nzs.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://brl.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://eht.sjlbkw.cn

[F09] 获取文件大小
来源：http://lto.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://cbg.fktsv.cn

PHP:  filesize("a.txt");
来源：http://dfj.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://qzu.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://brx.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://omz.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kik.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://qtk.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://zbh.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://zdu.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://har.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgu.yonumen.top


<!-- 参考信息 -->