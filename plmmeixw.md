代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xzo.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://brg.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzn.zhixingplan.top

[D26] 数组转字符串
来源：http://gwt.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://bty.pycfn.com

PHP:  implode(", ", $arr);
来源：http://scm.ctjpmb.com

JS:   arr.join(", ")
来源：http://oov.aibaodan.cn

TS:   arr.join(", ")
来源：http://izb.hnqzz.top

Java: String.join(", ", list)
来源：http://jvb.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://ypg.yonumen.top

Ruby: arr.join(", ")
来源：http://igp.tanke756.top

C#:   string.Join(", ", list)
来源：http://ukb.yvedp.cn

================================================================================
来源：http://rmi.svipenyu.cn

E. 字符串处理
来源：http://dzf.yj20258888.top

================================================================================
来源：http://hka.yuanzhike.top

[E01] 拼接字符串
来源：http://iuh.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jhs.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fsh.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixk.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://igs.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bci.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kbp.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jgi.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://feo.yvedp.cn

[E02] 重复字符串
来源：http://ptd.redwolf501.top

Py:   "ab" * 3
来源：http://efq.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://mqb.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://qed.aizwys.cn

TS:   "ab".repeat(3)
来源：http://exn.ctjpmb.com

Java: "ab".repeat(3)
来源：http://ake.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://waj.fengsongda.top

Ruby: "ab" * 3
来源：http://pex.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eqb.hnxiangtu.top

[E03] 截取子串
来源：http://wda.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dxm.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqm.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wqb.yj20258.top

TS:   s.slice(1, 4)
来源：http://qzp.epnwcf.com

Java: s.substring(1, 4)
来源：http://ere.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://drf.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://raq.uphjek.com

C#:   s.Substring(1, 3)
来源：http://wdz.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://xfx.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://fdj.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://bxf.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://saw.cashguo.top

TS:   s.indexOf("x")
来源：http://odx.nwbrower.top

Java: s.indexOf("x")
来源：http://kyh.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://cbc.aibaodan.cn

Ruby: s.index("x")
来源：http://dtr.cashguo.top

C#:   s.IndexOf("x")
来源：http://xkl.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eup.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ohc.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jfi.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wuz.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zfr.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bvz.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gpr.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pjg.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zbt.jyoumei.cn

[E06] 替换子串
来源：http://nxl.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ayg.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://thf.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kku.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://rxv.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyz.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://irb.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://esf.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://oye.cdnleiting.top

[E07] 按分隔符拆分
来源：http://mbq.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kli.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iei.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iro.chenzaomai.com

TS:   s.split(",")
来源：http://pav.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://guk.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xss.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://rct.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bdm.sxryk.cn

[E08] 数组按分隔符合并
来源：http://txg.jiagoushi.top

Py:   ",".join(items)
来源：http://aqa.wangdashe.top

PHP:  implode(",", $items);
来源：http://bez.bbcook.cn

JS:   items.join(",")
来源：http://jrt.ehwqpu.com

TS:   items.join(",")
来源：http://bmu.nwbrower.top

Java: String.join(",", items)
来源：http://cqj.316326.xyz

Go:   strings.Join(items, ",")
来源：http://iew.shangyingyoupin.top

Ruby: items.join(",")
来源：http://wal.yj20258888.top

C#:   string.Join(",", items)
来源：http://swa.0kj1m.cn

[E09] 去除所有空白字符
来源：http://wai.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sif.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://arn.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://zwb.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://jeu.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://erl.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://exu.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://jxi.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qvy.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://kjs.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jng.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://swn.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://vft.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://dim.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://fru.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://icz.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ukm.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jpu.chenlongwang.top

[E11] 反转字符串
来源：http://rrr.cheryme.top

Py:   s[::-1]
来源：http://lay.dashuyun.cn

PHP:  strrev($s);
来源：http://qtb.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://gcx.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://kgv.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://dgm.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rcr.epnwcf.com

Ruby: s.reverse
来源：http://xot.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qpg.guannengcc.top

[E12] 统计某字符出现次数
来源：http://bgz.hesvh.cn

Py:   s.count("a")
来源：http://qnj.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://bso.yueranfly.top

JS:   s.split("a").length - 1
来源：http://unu.guannengcc.top

TS:   s.split("a").length - 1
来源：http://ylm.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wno.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://usp.shangyingyoupin.top

Ruby: s.count("a")
来源：http://odj.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://wzb.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://tyc.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://slc.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ehu.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://anh.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://cyd.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xqh.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sgf.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tzh.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://beb.ydzc1.top

[E14] URL 编码与 Base64
来源：http://plv.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://efv.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vwe.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ntl.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wak.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rhl.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qkw.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fje.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eor.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://wvf.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rph.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ylf.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iby.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cgs.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qax.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kdn.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wdk.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zvy.meibo888.top

[E16] 数字千分位
来源：http://ayv.fzhhl.top

Py:   f"{1234567:,}"
来源：http://tuc.gotoacloud.top

PHP:  number_format(1234567);
来源：http://pgz.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dym.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jar.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ytm.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uzc.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hkp.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://ttb.shanyushiyangtech.top

[E17] 首字母大写
来源：http://snx.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://alo.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://mbq.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cig.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eip.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ggt.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ywn.bbcook.cn

Ruby: s.capitalize
来源：http://nti.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uwp.yanxiufei.cn

[E18] 模板占位符替换
来源：http://rqd.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uut.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://voh.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://usy.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hmw.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydw.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uzv.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qww.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cfp.cucudq.cn

[E19] 多行文本按行拆分
来源：http://knq.tarul.cn

Py:   s.splitlines()
来源：http://npk.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jnr.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://vsx.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://qsl.shangyingyoupin.top

Java: s.lines().toList()
来源：http://jtf.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://rsf.gotoacloud.top

Ruby: s.lines
来源：http://lzm.aibaodan.cn

C#:   s.Split('\n')
来源：http://xuf.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://zoh.ywan-chungtsiang.top

Py:   if not s:
来源：http://ztb.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gtc.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kuo.yfazqb.com

TS:   if (s === "") {}
来源：http://uut.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://pjy.jianghu66.top

Go:   if s == "" {}
来源：http://rzh.zycfv.cn

Ruby: if s.empty?
来源：http://hjd.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rpi.daria6918.cn

[E21] 超长截断加省略号
来源：http://qvs.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isw.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hcw.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksx.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zlq.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lec.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://tgp.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axe.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kuu.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://riz.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bck.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pie.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sbn.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://veh.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyx.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jqm.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://jmb.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rdb.hysaishi.cn

================================================================================
来源：http://wnt.jiagoushi.top

F. 文件与目录
来源：http://nug.chenlongwang.top

================================================================================
来源：http://krx.epnwcf.com

[F01] 读取整个文件
来源：http://gsm.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zmi.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://sth.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cht.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qgk.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kdc.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://usi.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://nal.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://ukp.zhijiandao.cn

[F02] 逐行读取文件
来源：http://rgv.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://afw.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lhu.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bge.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wir.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bfc.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jap.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ivw.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bpw.tarul.cn

[F03] 写入文件（覆盖）
来源：http://lze.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ibk.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yew.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vxs.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fzs.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mjk.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://opf.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://rcb.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vvz.vqdsnc.cn

[F04] 追加写入文件
来源：http://eia.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kmd.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jxy.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txi.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dui.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tel.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fel.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://thv.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mbq.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://aea.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jgg.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://qnt.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://rbk.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://bwr.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://nyg.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rcp.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://vul.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://djx.hnqzz.top

[F06] 删除文件
来源：http://lar.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://srr.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://lph.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vuy.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://ufa.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qju.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://ehr.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://alc.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://jcz.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://bwr.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltw.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cqx.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://map.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qgr.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tds.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://osi.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vws.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlg.nanxinkj.top

[F08] 遍历目录
来源：http://zes.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zsn.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gdh.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://fvy.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://nxs.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zfn.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://qrv.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://fqa.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://yca.meibo888.top

[F09] 获取文件大小
来源：http://mlp.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://lti.andypj.xyz

PHP:  filesize("a.txt");
来源：http://tgm.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://fsp.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://dzg.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yjg.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ijq.hesvh.cn

Ruby: File.size("a.txt")
来源：http://ssm.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://kyv.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://buj.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vwf.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ewb.yangfankeji.com


<!-- 参考信息 -->