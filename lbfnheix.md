代发 wailian999

TS:   "ab".repeat(3)
来源：http://zwe.aibaodan.cn

Java: "ab".repeat(3)
来源：http://ukw.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://crd.zdqjudy.top

Ruby: "ab" * 3
来源：http://qci.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xoi.fzhhl.top

[E03] 截取子串
来源：http://nmy.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xav.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kck.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jun.sxryk.cn

TS:   s.slice(1, 4)
来源：http://dql.daxiang520.top

Java: s.substring(1, 4)
来源：http://ozl.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://phr.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sjs.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://jps.cheryme.top

[E04] 查找子串位置
来源：http://cql.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://coe.mhx1999.top

PHP:  strpos($s, "x");
来源：http://hao.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wkf.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://plq.yuxming.cn

Java: s.indexOf("x")
来源：http://hib.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://vhy.kuanghao11.cn

Ruby: s.index("x")
来源：http://vth.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://udn.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ypr.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dbe.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qll.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ylu.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://tqr.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://prz.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tmm.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fib.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eic.snrcjt.cn

[E06] 替换子串
来源：http://iis.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://txl.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://nxe.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bnd.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://qwl.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxq.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oxc.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qjl.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://qmc.hnqzz.top

[E07] 按分隔符拆分
来源：http://xrp.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pbm.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fax.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sjt.9152youxi.cn

TS:   s.split(",")
来源：http://xfv.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fzd.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yny.hammf.cn

Ruby: s.split(",");  s.split
来源：http://nau.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oja.daria6918.cn

[E08] 数组按分隔符合并
来源：http://jhi.hnxiangtu.top

Py:   ",".join(items)
来源：http://ffo.guowangkeji.top

PHP:  implode(",", $items);
来源：http://mlo.yonumen.top

JS:   items.join(",")
来源：http://koo.fehbvm.com

TS:   items.join(",")
来源：http://ctg.gzhubu.top

Java: String.join(",", items)
来源：http://vra.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://iab.jqgufenzy.top

Ruby: items.join(",")
来源：http://mbm.guowangkeji.top

C#:   string.Join(",", items)
来源：http://crt.tarul.cn

[E09] 去除所有空白字符
来源：http://emz.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qng.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://crp.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://izh.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://vvx.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://jsz.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xil.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dzm.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uni.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://xec.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nsm.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zew.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://gvj.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://daz.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://mnp.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://pwb.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zlh.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nzr.sjlbkw.cn

[E11] 反转字符串
来源：http://upt.uphjek.com

Py:   s[::-1]
来源：http://yhm.zdqjudy.top

PHP:  strrev($s);
来源：http://dpa.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://gyq.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://srx.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rwy.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tcz.gaohongyu789.top

Ruby: s.reverse
来源：http://tsn.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rcx.daxiang520.top

[E12] 统计某字符出现次数
来源：http://luu.sjlbkw.cn

Py:   s.count("a")
来源：http://yyc.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://xlx.sxryk.cn

JS:   s.split("a").length - 1
来源：http://gic.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://hvy.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jkz.ivvv.top

Go:   strings.Count(s, "a")
来源：http://msl.52xcode.cn

Ruby: s.count("a")
来源：http://rqk.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://ugl.andypj.xyz

[E13] 逐字符遍历
来源：http://cga.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://nzz.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lrc.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://whd.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ukw.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rcq.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ezj.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kzr.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oel.birdmap.top

[E14] URL 编码与 Base64
来源：http://mfj.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxp.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://pns.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rwq.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xzi.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qce.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zxb.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nqv.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jrx.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://rot.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ldx.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aev.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bhp.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zek.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://izq.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zjk.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xlp.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cuz.tian-w.cn

[E16] 数字千分位
来源：http://gti.fktsv.cn

Py:   f"{1234567:,}"
来源：http://irr.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://yoq.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rit.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://shr.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lgd.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vgg.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cez.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://tko.ctjpmb.com

[E17] 首字母大写
来源：http://lvt.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cow.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uwb.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sjp.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tbp.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eej.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://inu.haohaochexian.top

Ruby: s.capitalize
来源：http://six.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xsd.zhixingplan.top

[E18] 模板占位符替换
来源：http://kms.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nnt.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://leg.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bah.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bpa.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rlk.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ago.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tji.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ikq.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://vzd.jlsjyb.cn

Py:   s.splitlines()
来源：http://ptp.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oee.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://fha.sweek.top

TS:   s.split(/\r?\n/)
来源：http://yaq.hnxiangtu.top

Java: s.lines().toList()
来源：http://mqq.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://wqt.ppjwa.cn

Ruby: s.lines
来源：http://cyc.birdmap.top

C#:   s.Split('\n')
来源：http://ocd.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://coe.zhoulong.xyz

Py:   if not s:
来源：http://nvy.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nio.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hdr.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://bae.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://eth.dashuyun.cn

Go:   if s == "" {}
来源：http://oxt.hesvh.cn

Ruby: if s.empty?
来源：http://dee.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://snl.shzxlz.cn

[E21] 超长截断加省略号
来源：http://tax.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uev.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iwa.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://icn.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ulp.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nbt.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://jnm.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ybc.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://egq.yj20258888.top

[E22] 字节长度与字符长度
来源：http://qnh.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://axt.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://icl.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qwa.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyf.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bev.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ovq.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://ccs.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fdq.jqgfzy.top

================================================================================
来源：http://dzj.tarul.cn

F. 文件与目录
来源：http://xod.aibaodan.cn

================================================================================
来源：http://sxk.hysaishi.cn

[F01] 读取整个文件
来源：http://jnn.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fru.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://skl.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gjl.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zah.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cek.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tos.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://fjj.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://zta.vehdjk.com

[F02] 逐行读取文件
来源：http://irm.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wrz.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cbk.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mck.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mph.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wqb.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kyb.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kbh.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nyl.havefunace.top

[F03] 写入文件（覆盖）
来源：http://tsw.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rls.mhx1999.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rbm.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pec.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ylf.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sro.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xba.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://siq.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qhh.fehbvm.com

[F04] 追加写入文件
来源：http://dxd.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aav.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hmr.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvm.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dht.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hqt.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vgy.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wam.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ele.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://jap.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iuk.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://ugh.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://ihk.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://yzn.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xru.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vha.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://wtg.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://bvh.fanxiaobao.xyz

[F06] 删除文件
来源：http://vaz.ybcxt.top

Py:   os.remove("a.txt")
来源：http://eck.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://tld.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://dhn.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://cle.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kpv.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://jpb.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://ydq.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://reg.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://zoi.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vjt.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aca.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oeb.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lia.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zug.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ovl.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rpb.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jwm.pycfn.com

[F08] 遍历目录
来源：http://hvr.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hsp.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kes.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://lqi.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://nhu.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rgn.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cnd.nwbrower.top

Ruby: Dir.children("dir")
来源：http://kxx.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://zpl.aibaodan.cn

[F09] 获取文件大小
来源：http://ija.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://bdx.fktsv.cn

PHP:  filesize("a.txt");
来源：http://cuh.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://gea.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://qwo.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tjh.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ekk.hesvh.cn

Ruby: File.size("a.txt")
来源：http://aur.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://awr.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://khm.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://scc.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bhp.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bsy.cashguo.top

TS:   path.extname("a.txt")
来源：http://gxi.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ydq.52xcode.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://spb.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gnf.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://njd.xylfe.cn

[F11] 复制与移动文件
来源：http://akp.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yic.xylfe.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rbb.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lgs.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ejm.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bti.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hef.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ccy.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ipx.jinqigufen.top

[F12] CSV 读写
来源：http://nak.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lke.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xdb.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lnv.zhixingplan.top

TS:   // 同上
来源：http://mrj.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aoa.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dej.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tnj.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wnv.shanyushiyangtech.top

================================================================================
来源：http://lmr.yuxming.cn

G. 面向对象
来源：http://bpc.hongshengwenyu.top

================================================================================
来源：http://jnn.jinyuanbaomall.cn

[G01] 定义类
来源：http://vsu.sysykeji.top


<!-- 参考信息 -->