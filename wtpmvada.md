代发 wailian999

================================================================================
来源：http://gaj.yongpay.top

E. 字符串处理
来源：http://zhw.xylfe.cn

================================================================================
来源：http://wqj.yj20258888.top

[E01] 拼接字符串
来源：http://ipc.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gcs.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ftt.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iwz.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vlq.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bsz.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cvs.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rdv.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdu.nanxinkj.top

[E02] 重复字符串
来源：http://vyr.fengsongda.top

Py:   "ab" * 3
来源：http://zva.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://una.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://bbi.hcnkem.com

TS:   "ab".repeat(3)
来源：http://dka.jinqigufen.top

Java: "ab".repeat(3)
来源：http://joi.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://nzt.0kj1m.cn

Ruby: "ab" * 3
来源：http://ycs.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wde.snrcjt.cn

[E03] 截取子串
来源：http://hjh.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zdr.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wgy.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rsd.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://ivd.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://hja.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bzy.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://lyb.yongpay.top

C#:   s.Substring(1, 3)
来源：http://rsy.chenlongwang.top

[E04] 查找子串位置
来源：http://gfa.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://chk.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://byt.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qdo.hywenlv.cn

TS:   s.indexOf("x")
来源：http://ubr.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://ohh.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://hdg.hysaishi.cn

Ruby: s.index("x")
来源：http://csv.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://vsx.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bfu.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rfc.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vgp.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iey.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ipd.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qhk.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kvu.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xka.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://srr.fehbvm.com

[E06] 替换子串
来源：http://eqg.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wyr.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://hsi.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://liy.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://zzp.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qwp.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://brt.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://szs.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://iix.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://oog.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iiu.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fwf.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rwz.yonumen.top

TS:   s.split(",")
来源：http://osj.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://phd.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ouf.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://wwh.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mdk.316326.xyz

[E08] 数组按分隔符合并
来源：http://cnz.chenlongwang.top

Py:   ",".join(items)
来源：http://gwl.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://ywz.gotoacloud.top

JS:   items.join(",")
来源：http://pam.hywenlv.cn

TS:   items.join(",")
来源：http://mek.xuanzx.com

Java: String.join(",", items)
来源：http://slm.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://xws.jiagoushi.top

Ruby: items.join(",")
来源：http://szj.guowangkeji.top

C#:   string.Join(",", items)
来源：http://ejy.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://kgz.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pfb.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lni.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://uqi.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://vgg.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://edz.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xkx.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qkc.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ezh.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://wgm.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zus.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bzu.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://lpo.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://org.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://squ.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://egz.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://icq.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jee.mhx1999.top

[E11] 反转字符串
来源：http://cyj.quarkkingdee.top

Py:   s[::-1]
来源：http://smr.ppjwa.cn

PHP:  strrev($s);
来源：http://cmt.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://iex.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://las.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://rll.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yuw.fanxiaobao.xyz

Ruby: s.reverse
来源：http://xbj.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pmk.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://ivv.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://euy.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://jht.pycfn.com

JS:   s.split("a").length - 1
来源：http://xxa.tarul.cn

TS:   s.split("a").length - 1
来源：http://cav.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lvz.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://llu.tian-w.cn

Ruby: s.count("a")
来源：http://rxy.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://lft.shzxlz.cn

[E13] 逐字符遍历
来源：http://dnw.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://mxv.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ixd.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vay.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://juh.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oso.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tfr.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pmw.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bbe.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://itt.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pvb.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lcw.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://khc.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://psp.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://evi.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drl.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://crl.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pej.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://ste.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yuz.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fxh.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gtb.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bvu.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qyu.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bnm.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://trz.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://puh.hesvh.cn

[E16] 数字千分位
来源：http://fgq.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://bqa.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://dff.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://enw.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://syc.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ita.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cny.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aya.cheryme.top

C#:   1234567.ToString("N0")
来源：http://mws.svipenyu.cn

[E17] 首字母大写
来源：http://mbi.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wxq.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://akm.pycfn.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zlj.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aib.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qnd.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://skf.shangyingyoupin.top

Ruby: s.capitalize
来源：http://jsr.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zab.vqdsnc.cn

[E18] 模板占位符替换
来源：http://ubs.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tcb.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mas.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tkc.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uhr.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fkl.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gvo.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vyu.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://brs.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://vwv.andypj.xyz

Py:   s.splitlines()
来源：http://ajf.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ndd.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://zmn.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://ovv.andypj.xyz

Java: s.lines().toList()
来源：http://lhb.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://bye.dashuyun.cn

Ruby: s.lines
来源：http://yov.tian-w.cn

C#:   s.Split('\n')
来源：http://sya.bbcook.cn

[E20] 判断字符串是否为空
来源：http://vbu.fanxiaobao.xyz

Py:   if not s:
来源：http://ktw.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rcf.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hla.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://cul.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://aos.daria6918.cn

Go:   if s == "" {}
来源：http://dli.0kj1m.cn

Ruby: if s.empty?
来源：http://lao.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nmd.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://lzh.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nbh.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tng.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oek.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nhe.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ash.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://ovp.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ysc.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iya.fehbvm.com

[E22] 字节长度与字符长度
来源：http://rhf.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zuu.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://omj.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dvc.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcl.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iaf.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jgi.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://ksk.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kta.snrcjt.cn

================================================================================
来源：http://zhk.hysaishi.cn

F. 文件与目录
来源：http://jtv.yongpay.top

================================================================================
来源：http://prh.gzhubu.top

[F01] 读取整个文件
来源：http://cbu.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ftg.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://uyi.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gaa.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wxo.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nzw.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fnm.fzhhl.top

Ruby: File.read("a.txt")
来源：http://qlb.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://ejv.chenzaomai.com

[F02] 逐行读取文件
来源：http://mfr.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iiq.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tzz.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kaz.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iyc.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hgx.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zki.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://phc.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zqe.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://cwu.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jnc.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fde.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zdb.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dtx.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tcb.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nqy.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://ldt.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vms.chenjidiqi.icu

[F04] 追加写入文件
来源：http://ixi.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jaf.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ggr.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://arv.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjp.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kah.zhiwuduotai.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://snp.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xpd.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://itq.uphjek.com

[F05] 判断文件或目录是否存在
来源：http://het.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yhw.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://joq.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://osr.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://rcq.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mxl.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wcs.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://ncz.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://jac.bbcook.cn

[F06] 删除文件
来源：http://gyi.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://qfa.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://gov.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dkv.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://ffp.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eyz.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://kks.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://sww.316326.xyz

C#:   File.Delete("a.txt");
来源：http://ofh.52xcode.cn

[F07] 创建目录（含多级）
来源：http://eno.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yny.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wsd.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgb.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nib.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nxj.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xgk.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dqe.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://puz.fzhhl.top

[F08] 遍历目录
来源：http://tfg.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dwh.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bkp.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://vpt.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://vmn.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mvg.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mqi.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://lrj.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://tpf.316326.xyz

[F09] 获取文件大小
来源：http://ots.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://cjj.birdmap.top

PHP:  filesize("a.txt");
来源：http://rql.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://xge.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://nav.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dlt.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fxg.bbcook.cn

Ruby: File.size("a.txt")
来源：http://wzf.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://pho.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://xjt.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://evk.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aia.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nkx.bjfxy.top

TS:   path.extname("a.txt")
来源：http://tgl.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ady.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fic.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yaq.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mco.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://spw.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kip.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vvb.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tna.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hdq.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://onn.hcnkem.com


<!-- 参考信息 -->