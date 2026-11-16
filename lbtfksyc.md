代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://atc.yongpay.top

[E03] 截取子串
来源：http://fas.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aop.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bch.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://piy.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://qnj.ydzc1.top

Java: s.substring(1, 4)
来源：http://oej.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hlh.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lvg.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://sez.mhx1999.top

[E04] 查找子串位置
来源：http://ors.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://ayh.havefunace.top

PHP:  strpos($s, "x");
来源：http://sft.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yvd.zycfv.cn

TS:   s.indexOf("x")
来源：http://dec.shuidangran.top

Java: s.indexOf("x")
来源：http://kat.yongpay.top

Go:   strings.Index(s, "x")
来源：http://gxg.cashguo.top

Ruby: s.index("x")
来源：http://nci.gzhubu.top

C#:   s.IndexOf("x")
来源：http://xtj.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://slg.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kgv.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gun.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://izv.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://hbz.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmb.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hbn.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vst.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gyl.gotoacloud.top

[E06] 替换子串
来源：http://yfp.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vmf.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://cah.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggq.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://xkd.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xwt.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tab.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://czj.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://rhf.shzxlz.cn

[E07] 按分隔符拆分
来源：http://efo.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aox.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://evt.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://alk.cucudq.cn

TS:   s.split(",")
来源：http://wiv.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://oeg.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tho.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://wxy.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wse.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://okb.chenjidiqi.icu

Py:   ",".join(items)
来源：http://lnm.tianlin.xyz

PHP:  implode(",", $items);
来源：http://axc.zhiwuduotai.top

JS:   items.join(",")
来源：http://rwc.jiagoushi.top

TS:   items.join(",")
来源：http://yay.gzhubu.top

Java: String.join(",", items)
来源：http://hhh.havefunace.top

Go:   strings.Join(items, ",")
来源：http://epu.fehbvm.com

Ruby: items.join(",")
来源：http://flb.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://xvu.sysykeji.top

[E09] 去除所有空白字符
来源：http://zkh.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yjl.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://buu.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://vcg.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://rbv.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://auf.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lya.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://bmz.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://phn.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://fyi.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nmm.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ncg.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://omw.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://kqt.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://goj.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hvj.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hos.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xqq.hongshengwenyu.top

[E11] 反转字符串
来源：http://khn.wangshuangyany.cn

Py:   s[::-1]
来源：http://cha.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://zpv.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://rgf.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://xkb.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nej.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ofp.hnqzz.top

Ruby: s.reverse
来源：http://kab.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://ftd.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://viw.zdqjudy.top

Py:   s.count("a")
来源：http://ajg.hammf.cn

PHP:  substr_count($s, "a");
来源：http://zae.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://vsk.bjfxy.top

TS:   s.split("a").length - 1
来源：http://deu.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cpf.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://blf.hnxiangtu.top

Ruby: s.count("a")
来源：http://zwi.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://xpf.bjfxy.top

[E13] 逐字符遍历
来源：http://dyw.havefunace.top

Py:   for ch in s: print(ch)
来源：http://mcx.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ffq.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xsa.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://zcd.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fyb.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vxi.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hio.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fav.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://vqy.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kph.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://orh.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uei.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vnh.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bww.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cob.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rnk.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qxg.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://pzh.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://abz.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kuu.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xqi.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cbl.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wsz.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ibo.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jkc.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vbk.zhixingplan.top

[E16] 数字千分位
来源：http://mrq.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://slp.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://hcd.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pvf.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://wlp.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wnb.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://quh.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pbt.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://hvr.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://ajg.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vht.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://prh.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://njf.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsq.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dth.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://igi.yonumen.top

Ruby: s.capitalize
来源：http://mns.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gkc.svipenyu.cn

[E18] 模板占位符替换
来源：http://jcp.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rgc.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vbr.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rel.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://anv.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gnf.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qxp.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uzo.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ely.bjfxy.top

[E19] 多行文本按行拆分
来源：http://ydc.cashguo.top

Py:   s.splitlines()
来源：http://bqr.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://awb.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://odb.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://fwl.316326.xyz

Java: s.lines().toList()
来源：http://tzo.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://lgg.shangyingyoupin.top

Ruby: s.lines
来源：http://nnh.uphjek.com

C#:   s.Split('\n')
来源：http://sjc.tian-w.cn

[E20] 判断字符串是否为空
来源：http://coo.gogol.net.cn

Py:   if not s:
来源：http://xry.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wcz.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wha.sweek.top

TS:   if (s === "") {}
来源：http://haa.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://qcw.ydzc1.top

Go:   if s == "" {}
来源：http://nmw.quarkkingdee.top

Ruby: if s.empty?
来源：http://phv.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ylq.yueranfly.top

[E21] 超长截断加省略号
来源：http://fzs.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lbs.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hfv.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqa.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ett.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lrr.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://bnz.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bad.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://itu.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://aek.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kxy.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hgu.jinqigfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kar.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkl.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bdc.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lee.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://arp.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dww.tanke756.top

================================================================================
来源：http://kvb.yj20258888.top

F. 文件与目录
来源：http://skt.mhx1999.top

================================================================================
来源：http://btw.tarul.cn

[F01] 读取整个文件
来源：http://opb.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rmf.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://nxr.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jnc.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rbr.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rgm.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://crt.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://vbt.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://nse.vehdjk.com

[F02] 逐行读取文件
来源：http://wux.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jsv.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://slb.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bxd.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cmq.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://psp.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://liv.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://itj.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fyf.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://qrx.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hxc.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qis.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xkb.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yhq.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vuh.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jqv.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://def.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://npx.zhijiandao.cn

[F04] 追加写入文件
来源：http://fgu.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tow.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kio.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qkt.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pzk.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jdb.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dkw.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yve.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yga.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://vsm.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wax.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://gvp.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://gdk.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://mvx.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wov.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nza.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://rbb.hammf.cn

C#:   File.Exists("a.txt")
来源：http://dnd.tanke756.top

[F06] 删除文件
来源：http://fth.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://dqa.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://nal.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://jex.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hfq.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yve.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://ppg.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://okx.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://ctr.pycfn.com

[F07] 创建目录（含多级）
来源：http://nva.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jkq.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bkb.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://frc.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pao.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zmc.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lki.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rnz.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xvm.ivvv.top

[F08] 遍历目录
来源：http://vjy.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sgv.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sct.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://npv.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://dlx.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://whw.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://caw.shuidangran.top

Ruby: Dir.children("dir")
来源：http://sna.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://epy.bbcook.cn

[F09] 获取文件大小
来源：http://tft.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://oea.xinyue.icu

PHP:  filesize("a.txt");
来源：http://gkd.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://len.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://jcc.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zzw.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://shv.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://uet.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://qqg.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://hdt.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nyp.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cue.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mok.shuidangran.top

TS:   path.extname("a.txt")
来源：http://ksa.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qgy.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://znn.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gax.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sng.daxiang520.top

[F11] 复制与移动文件
来源：http://rqt.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzv.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mnk.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gnd.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rnb.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vfa.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xbt.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zjw.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aga.aizwys.cn

[F12] CSV 读写
来源：http://dnn.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fzv.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xcx.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hwa.zhiwuduotai.top

TS:   // 同上
来源：http://sus.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qci.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sie.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ntc.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://xfb.aizwys.cn

================================================================================
来源：http://zxs.gzhubu.top

G. 面向对象
来源：http://kph.jinqigfzy.top

================================================================================
来源：http://qgp.jyoumei.cn

[G01] 定义类
来源：http://hki.9152youxi.cn

Py:   class User: pass
来源：http://epw.jianghu66.top

PHP:  class User {}
来源：http://vfi.shuidangran.top

JS:   class User {}
来源：http://iin.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://gnp.xuanzx.com


<!-- 参考信息 -->