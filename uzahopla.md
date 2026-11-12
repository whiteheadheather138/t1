代发 wailian999

PHP:  strpos($s, "x");
来源：http://deg.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zzr.bbcook.cn

TS:   s.indexOf("x")
来源：http://lvv.jiagoushi.top

Java: s.indexOf("x")
来源：http://roz.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://yvq.zhixingplan.top

Ruby: s.index("x")
来源：http://scp.cashguo.top

C#:   s.IndexOf("x")
来源：http://afw.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sww.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mgc.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hsr.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mut.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sfb.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wwa.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://olx.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zch.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nfw.shuidangran.top

[E06] 替换子串
来源：http://qkr.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jvj.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://cil.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rqj.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://bxo.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qrt.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tqh.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mgv.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://lnx.52xcode.cn

[E07] 按分隔符拆分
来源：http://onx.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rag.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vnl.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tkv.sxryk.cn

TS:   s.split(",")
来源：http://ssf.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://gzm.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://juu.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://xnp.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uji.xinyue.icu

[E08] 数组按分隔符合并
来源：http://rzs.316326.xyz

Py:   ",".join(items)
来源：http://tkt.yfazqb.com

PHP:  implode(",", $items);
来源：http://vzm.snrcjt.cn

JS:   items.join(",")
来源：http://gzt.yj20258.top

TS:   items.join(",")
来源：http://iot.mhx1999.top

Java: String.join(",", items)
来源：http://hpb.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://mbi.yonumen.top

Ruby: items.join(",")
来源：http://xlt.hysaishi.cn

C#:   string.Join(",", items)
来源：http://hxn.cheryme.top

[E09] 去除所有空白字符
来源：http://cmc.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mbt.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ooh.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://fdz.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://add.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://vsp.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://llx.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qni.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bnq.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://glq.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jwv.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mem.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://wje.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://iiw.andypj.xyz

Java: String.format("%03d", 7)
来源：http://vtt.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://umr.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yzh.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uep.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://wpf.sufxvd.cn

Py:   s[::-1]
来源：http://ywl.pycfn.com

PHP:  strrev($s);
来源：http://jre.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://tse.yonumen.top

TS:   [...s].reverse().join("")
来源：http://rkv.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://fmx.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xqp.chenlongwang.top

Ruby: s.reverse
来源：http://smx.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hrp.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://jcv.daria6918.cn

Py:   s.count("a")
来源：http://xfy.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://zzv.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://tvi.daria6918.cn

TS:   s.split("a").length - 1
来源：http://wzt.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xvx.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://kru.wangshuangyany.cn

Ruby: s.count("a")
来源：http://egz.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://ehn.sysykeji.top

[E13] 逐字符遍历
来源：http://fzo.yongpay.top

Py:   for ch in s: print(ch)
来源：http://jyl.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kdx.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wrj.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jhb.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kad.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://npf.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uoa.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jzy.tanke756.top

[E14] URL 编码与 Base64
来源：http://wrs.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://frc.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kcc.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xvd.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohk.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rtl.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lxc.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://amx.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cps.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://ncz.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zwp.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qpq.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ara.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lfj.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sjp.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sbb.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://quc.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yty.dashuyun.cn

[E16] 数字千分位
来源：http://xbn.fehbvm.com

Py:   f"{1234567:,}"
来源：http://cnj.smart0.xyz

PHP:  number_format(1234567);
来源：http://tny.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mpr.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yxb.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ovu.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wyq.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rly.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://knf.smart0.xyz

[E17] 首字母大写
来源：http://ydu.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vbt.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://job.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zdi.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vun.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bcb.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bij.vqdsnc.cn

Ruby: s.capitalize
来源：http://pzj.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pdb.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://xfn.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ynw.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://olh.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uhs.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fjm.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dni.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klw.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dsv.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xcl.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://cjg.bbcook.cn

Py:   s.splitlines()
来源：http://jbq.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kaq.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://pnq.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://akc.nanxuanxn.top

Java: s.lines().toList()
来源：http://fxj.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://lis.yuxming.cn

Ruby: s.lines
来源：http://vsm.guowangkeji.top

C#:   s.Split('\n')
来源：http://ywb.tian-w.cn

[E20] 判断字符串是否为空
来源：http://gjk.ywan-chungtsiang.top

Py:   if not s:
来源：http://lej.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jmx.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hwj.aibaodan.cn

TS:   if (s === "") {}
来源：http://urj.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://gpm.zhongyouzk.top

Go:   if s == "" {}
来源：http://zib.hesvh.cn

Ruby: if s.empty?
来源：http://ild.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iri.gogol.net.cn

[E21] 超长截断加省略号
来源：http://frs.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ghr.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dby.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dyz.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fty.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://atb.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://pxt.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://joo.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcl.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://arr.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hwx.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jgj.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://szb.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iab.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cdl.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ktc.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://mcd.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kpr.zhaomingkeji.xyz

================================================================================
来源：http://ten.hfpthk.cn

F. 文件与目录
来源：http://quu.jyoumei.cn

================================================================================
来源：http://fel.sjlbkw.cn

[F01] 读取整个文件
来源：http://amq.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nju.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://sae.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rrj.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zty.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zjq.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ywn.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://gmi.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://edm.quarkkingdee.top

[F02] 逐行读取文件
来源：http://jud.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hfm.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dyf.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mxv.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vya.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wqs.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xcj.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xel.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oxe.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://wag.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zpn.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ulf.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgc.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cve.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vpi.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ucp.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://wlr.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hnw.shuidangran.top

[F04] 追加写入文件
来源：http://ait.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uoj.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zrp.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mlf.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://anx.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dif.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vru.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ntw.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kok.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://ytf.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bhw.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://otx.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://ajd.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://wno.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zfm.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nmc.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://rvx.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://gln.cdnleiting.top

[F06] 删除文件
来源：http://rod.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://eca.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://bjj.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://auy.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xii.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://var.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://xss.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://ynv.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://arv.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://kyp.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hjk.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sdx.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tsx.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bgk.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pbn.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qod.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rtl.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dsd.chenjidiqi.icu

[F08] 遍历目录
来源：http://vku.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rye.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jpu.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://nvq.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://mgi.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://myl.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oew.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://lnj.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://phn.0kj1m.cn

[F09] 获取文件大小
来源：http://tvc.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://asn.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://xop.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://qtk.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://awg.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://cly.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://djc.hesvh.cn

Ruby: File.size("a.txt")
来源：http://zgy.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://tzp.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://mvu.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mal.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mji.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rwf.hesvh.cn

TS:   path.extname("a.txt")
来源：http://ywb.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cnr.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gcl.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zmw.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eae.tianlin.xyz

[F11] 复制与移动文件
来源：http://aln.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cfj.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wtb.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jvr.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fpk.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jss.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dng.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://csj.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cdm.ydjk.org.cn

[F12] CSV 读写
来源：http://obn.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cuj.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zen.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mez.yj202588.top

TS:   // 同上
来源：http://wec.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oat.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://phh.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mos.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xnm.jinqigfzy.top

================================================================================
来源：http://xfk.fktsv.cn

G. 面向对象
来源：http://ors.shuidangran.top

================================================================================
来源：http://box.yvedp.cn

[G01] 定义类
来源：http://uxx.bjfxy.top

Py:   class User: pass
来源：http://xvm.ivvv.top

PHP:  class User {}
来源：http://xry.fengsongda.top

JS:   class User {}
来源：http://lnx.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://qdi.chenlongwang.top

Java: class User {}
来源：http://nqt.shuidangran.top

Go:   type User struct { Name string }
来源：http://eme.zhaomingkeji.xyz

Ruby: class User; end
来源：http://wkg.chenlongwang.top

C#:   class User {}
来源：http://gtz.xuetiantiany.cn

[G02] 构造函数
来源：http://erq.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://nuc.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://wwl.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://ryy.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://sfu.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://ipc.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://chx.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://vgc.pengpengdd.cyou


<!-- 参考信息 -->