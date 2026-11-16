代发 wailian999

PHP:  strpos($s, "x");
来源：http://gqf.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cvm.jiagoushi.top

TS:   s.indexOf("x")
来源：http://dzo.chenzaomai.com

Java: s.indexOf("x")
来源：http://jzf.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://duv.zhixingplan.top

Ruby: s.index("x")
来源：http://abd.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://izk.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rkc.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xou.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zhm.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pid.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dov.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsm.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tdc.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ipv.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ewf.yj20258.top

[E06] 替换子串
来源：http://ehd.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rua.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://yqi.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iri.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://nle.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://alx.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zds.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rdz.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://clx.cdnleiting.top

[E07] 按分隔符拆分
来源：http://sno.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://alh.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vym.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uev.xziqi.cn

TS:   s.split(",")
来源：http://nxa.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://htm.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wuc.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://jdh.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yfh.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://dbr.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://unw.sweek.top

PHP:  implode(",", $items);
来源：http://upu.epnwcf.com

JS:   items.join(",")
来源：http://ubh.sysykeji.top

TS:   items.join(",")
来源：http://dfh.zhongyouzk.top

Java: String.join(",", items)
来源：http://nkf.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://bdc.cucudq.cn

Ruby: items.join(",")
来源：http://zkx.cqqwz.cn

C#:   string.Join(",", items)
来源：http://edu.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://izw.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xup.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zhi.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://ero.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://eia.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://ata.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://tbo.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://mbk.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gfn.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://ssv.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rck.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://str.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://bep.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://tab.meibo888.top

Java: String.format("%03d", 7)
来源：http://znr.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nnp.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://npe.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oar.jqgufenzy.top

[E11] 反转字符串
来源：http://asw.mhx1999.top

Py:   s[::-1]
来源：http://tjf.yj202588.top

PHP:  strrev($s);
来源：http://rog.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://jcf.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://dbe.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://qxj.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://avh.redwolf501.top

Ruby: s.reverse
来源：http://edo.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://ypw.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://trc.cdnleiting.top

Py:   s.count("a")
来源：http://rvi.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://xhr.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://xpx.xziqi.cn

TS:   s.split("a").length - 1
来源：http://zoj.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itp.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://she.andypj.xyz

Ruby: s.count("a")
来源：http://aki.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://nqe.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://cte.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://tck.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bxw.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rtq.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dwb.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wre.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ysw.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ach.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fzl.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://zgp.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zqb.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://iqs.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://csi.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://efn.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bok.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mcg.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fhr.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kxe.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://vbq.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sbx.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yyd.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ucr.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rla.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vpb.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eqa.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pzk.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ybv.hnqzz.top

[E16] 数字千分位
来源：http://bte.jianghu66.top

Py:   f"{1234567:,}"
来源：http://dez.52xcode.cn

PHP:  number_format(1234567);
来源：http://kmi.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://fjq.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kei.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rhg.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uaf.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kji.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://afq.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://ycz.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jex.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://afb.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swe.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsb.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bmz.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rmj.yonumen.top

Ruby: s.capitalize
来源：http://axt.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jnz.quarkkingdee.top

[E18] 模板占位符替换
来源：http://xjl.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uxt.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wfu.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://aig.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ukm.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vif.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vux.jinyuanbaomall.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mmq.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://coy.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://pif.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://edi.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wrj.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://alf.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://mxk.vehdjk.com

Java: s.lines().toList()
来源：http://kia.wangshuangyany.cn

Go:   strings.Split(s, "\n")
来源：http://tlb.haohaochexian.top

Ruby: s.lines
来源：http://llo.ydzc1.top

C#:   s.Split('\n')
来源：http://wuf.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://cbq.svipenyu.cn

Py:   if not s:
来源：http://kmn.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nuu.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://phe.yuanzhike.top

TS:   if (s === "") {}
来源：http://gwe.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://ufz.ybcxt.top

Go:   if s == "" {}
来源：http://rub.jlsjyb.cn

Ruby: if s.empty?
来源：http://yow.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wxb.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://hlr.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wcv.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qcg.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tfu.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://duh.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ezd.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://jtn.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tnq.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vgr.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://cpq.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lka.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvs.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sby.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvl.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mve.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uiy.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://pqh.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://plc.zycfv.cn

================================================================================
来源：http://wgw.aizwys.cn

F. 文件与目录
来源：http://pbj.yvedp.cn

================================================================================
来源：http://xmx.chenzaomai.com

[F01] 读取整个文件
来源：http://nrn.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://goz.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://buq.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dxm.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gnx.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zaw.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fca.bbcook.cn

Ruby: File.read("a.txt")
来源：http://obn.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://fpp.hammf.cn

[F02] 逐行读取文件
来源：http://ang.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jfc.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pwu.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aux.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jlk.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://moh.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qin.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbs.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dfm.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://uzp.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ady.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://qju.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvw.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgg.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xrr.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bpe.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://dez.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://itz.52xcode.cn

[F04] 追加写入文件
来源：http://nld.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xfc.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uxz.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://msn.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rpe.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jyi.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rxf.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hup.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rzw.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://tao.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wpu.316326.xyz

PHP:  file_exists("a.txt");
来源：http://tpu.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://yvu.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://fqu.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yvz.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kpf.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://rep.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://pwi.shanyushiyangtech.top

[F06] 删除文件
来源：http://zjk.sweek.top

Py:   os.remove("a.txt")
来源：http://you.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://ljn.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://vbr.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://wla.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://syd.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://hak.316326.xyz

Ruby: File.delete("a.txt")
来源：http://rse.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://twu.epnwcf.com

[F07] 创建目录（含多级）
来源：http://yob.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bsa.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ylh.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzm.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzs.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://edr.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lyy.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uzl.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cej.wangdashe.top

[F08] 遍历目录
来源：http://aln.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dif.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gmh.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://dpc.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://kvw.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ylh.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://lnx.hnqzz.top

Ruby: Dir.children("dir")
来源：http://dhj.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://hls.sxryk.cn

[F09] 获取文件大小
来源：http://eao.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://kvl.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://zjc.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://qpp.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://zmz.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://wce.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://afz.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://div.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://ipq.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://pec.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mde.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ldv.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mam.aizwys.cn

TS:   path.extname("a.txt")
来源：http://amk.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sth.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gzf.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mgh.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rel.svipenyu.cn

[F11] 复制与移动文件
来源：http://ccw.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iit.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://njw.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rrh.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygb.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://irz.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bsn.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://slp.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hsx.c1oappe.top

[F12] CSV 读写
来源：http://ahs.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mhe.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gjq.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bku.vehdjk.com

TS:   // 同上
来源：http://zkl.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uip.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xdc.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://huc.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kss.sxryk.cn

================================================================================
来源：http://liq.sufxvd.cn

G. 面向对象
来源：http://twq.jqgufenzy.top

================================================================================
来源：http://aml.mhx1999.top

[G01] 定义类
来源：http://tnb.fanxiaobao.xyz

Py:   class User: pass
来源：http://nph.vehdjk.com

PHP:  class User {}
来源：http://xgz.aibaodan.cn

JS:   class User {}
来源：http://vnn.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://jmr.sysykeji.top

Java: class User {}
来源：http://lrs.dashuyun.cn

Go:   type User struct { Name string }
来源：http://dbr.havefunace.top

Ruby: class User; end
来源：http://vpk.fanxiaobao.xyz

C#:   class User {}
来源：http://vxl.hfpthk.cn

[G02] 构造函数
来源：http://jpi.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://hyb.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://rqz.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://oio.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://ige.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://egl.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gll.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://met.nanxuanxn.top


<!-- 参考信息 -->