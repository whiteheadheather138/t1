代发 wailian999

TS:   "ab".repeat(3)
来源：http://tri.shuidangran.top

Java: "ab".repeat(3)
来源：http://nfg.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://spf.hammf.cn

Ruby: "ab" * 3
来源：http://fsj.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://agy.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://iep.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cpj.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gca.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvg.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://qat.nanxinkj.top

Java: s.substring(1, 4)
来源：http://guo.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hov.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ear.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://fph.yongpay.top

[E04] 查找子串位置
来源：http://cek.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://nwf.hesvh.cn

PHP:  strpos($s, "x");
来源：http://eea.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://txg.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://lof.gaohongyu789.top

Java: s.indexOf("x")
来源：http://dcz.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://zsa.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://igk.xinyue.icu

C#:   s.IndexOf("x")
来源：http://aan.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cyx.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://imq.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jer.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vuw.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cya.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gog.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jde.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ggf.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kdg.nwbrower.top

[E06] 替换子串
来源：http://dvi.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://joh.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://bwp.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cav.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://smr.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yqu.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uyh.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wpu.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://cmo.zhixingplan.top

[E07] 按分隔符拆分
来源：http://aqb.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wzt.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lzj.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://icl.xinyue.icu

TS:   s.split(",")
来源：http://mnm.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://ouo.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://avr.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://raj.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wmh.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://lre.52xcode.cn

Py:   ",".join(items)
来源：http://twm.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://cmp.ydzc1.top

JS:   items.join(",")
来源：http://adp.tian-w.cn

TS:   items.join(",")
来源：http://glr.tianlin.xyz

Java: String.join(",", items)
来源：http://cwh.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://ret.yonumen.top

Ruby: items.join(",")
来源：http://kyd.yj202588.top

C#:   string.Join(",", items)
来源：http://piv.gzhubu.top

[E09] 去除所有空白字符
来源：http://xie.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wba.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wrw.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://ytu.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://kbm.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://lei.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://gqf.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://txu.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zrb.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://aua.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sos.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tjy.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://ski.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://tvo.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://tat.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://atm.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rpj.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://szf.hnxiangtu.top

[E11] 反转字符串
来源：http://lqw.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://mfi.guowangkeji.top

PHP:  strrev($s);
来源：http://dtb.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://pks.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://qic.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rsd.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hiq.daxiang520.top

Ruby: s.reverse
来源：http://dhh.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://bww.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://rag.andypj.xyz

Py:   s.count("a")
来源：http://los.cheryme.top

PHP:  substr_count($s, "a");
来源：http://llj.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://joc.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://ttn.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://njt.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://qhb.ivvv.top

Ruby: s.count("a")
来源：http://pyj.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://gox.uphjek.com

[E13] 逐字符遍历
来源：http://xiy.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://esd.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bnv.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tzu.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kid.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zvk.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fof.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sgx.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dso.hammf.cn

[E14] URL 编码与 Base64
来源：http://xao.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ghw.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aca.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fwe.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zsj.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mud.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cmz.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yzd.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://olb.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://aar.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pcy.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yrq.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hfl.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qnu.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nbo.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rqd.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://erp.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nlh.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://ass.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://zif.xylfe.cn

PHP:  number_format(1234567);
来源：http://lxw.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lgi.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nwd.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ihj.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xrd.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wxp.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://okt.vqdsnc.cn

[E17] 首字母大写
来源：http://qmh.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://skk.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fds.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zuy.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hvx.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mfs.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rqb.hongshengwenyu.top

Ruby: s.capitalize
来源：http://xpz.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nyd.sweek.top

[E18] 模板占位符替换
来源：http://vwc.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xnh.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bxm.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fct.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wdv.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rzc.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uir.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlp.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aqs.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://irh.0kj1m.cn

Py:   s.splitlines()
来源：http://rmf.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zdp.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://avu.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://wsl.hammf.cn

Java: s.lines().toList()
来源：http://rxl.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://lli.epnwcf.com

Ruby: s.lines
来源：http://wrt.mhx1999.top

C#:   s.Split('\n')
来源：http://ovx.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://eil.iojbl.cn

Py:   if not s:
来源：http://jgp.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://chn.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aan.zhoulong.xyz

TS:   if (s === "") {}
来源：http://fzj.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://eqm.hammf.cn

Go:   if s == "" {}
来源：http://wap.mhx1999.top

Ruby: if s.empty?
来源：http://uli.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ysr.yongpay.top

[E21] 超长截断加省略号
来源：http://yzo.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://itu.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iwy.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wke.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://est.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vmw.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://jgo.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jym.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lju.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://pha.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vkm.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sen.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kjh.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xli.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vpz.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cds.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://gyd.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zkn.zhijiandao.cn

================================================================================
来源：http://kij.yj202588.top

F. 文件与目录
来源：http://kxb.zhiwuduotai.top

================================================================================
来源：http://jsh.nanxuanxn.top

[F01] 读取整个文件
来源：http://bko.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yhh.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://ayt.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://szf.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mhu.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qsl.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ein.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://umd.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://qto.vqdsnc.cn

[F02] 逐行读取文件
来源：http://eov.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dxc.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nry.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gyg.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmq.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://knw.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xyo.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cmx.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jcp.pycfn.com

[F03] 写入文件（覆盖）
来源：http://znc.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sjn.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ton.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xpj.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://knl.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dzs.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xpa.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://yds.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pdj.ehwqpu.com

[F04] 追加写入文件
来源：http://fuf.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://saq.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qmd.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://abx.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://adz.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://red.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://abr.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ude.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nlc.sweek.top

[F05] 判断文件或目录是否存在
来源：http://fhu.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gif.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://xdf.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://rra.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://fuo.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lbk.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xhq.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://gil.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://zld.yueranfly.top

[F06] 删除文件
来源：http://fky.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://gsi.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://hcs.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://ppc.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://hft.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mxm.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://ihp.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://ecy.cashguo.top

C#:   File.Delete("a.txt");
来源：http://nem.bbcook.cn

[F07] 创建目录（含多级）
来源：http://gzh.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mjn.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hjr.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qcr.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mqo.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://akr.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xin.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hpr.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gjr.wangdashe.top

[F08] 遍历目录
来源：http://gaq.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ewg.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eif.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://bvl.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://xxj.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kpw.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cvd.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://rrx.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://dtu.sysykeji.top

[F09] 获取文件大小
来源：http://mcq.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://iis.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://voy.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://unj.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://jyi.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://eyk.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://trb.xinyue.icu

Ruby: File.size("a.txt")
来源：http://lnm.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://cmp.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://oru.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fgu.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kdd.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pbu.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://wnd.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://udb.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hik.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fas.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bsr.ybcxt.top

[F11] 复制与移动文件
来源：http://jaa.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bkg.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rwq.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xaw.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wme.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://okc.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xxn.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://imc.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uyx.aizwys.cn

[F12] CSV 读写
来源：http://okx.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vdb.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nnk.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fif.fzhhl.top

TS:   // 同上
来源：http://ugq.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hqs.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qcn.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ngs.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ism.hnqzz.top

================================================================================
来源：http://zjo.bbcook.cn

G. 面向对象
来源：http://chl.zdqjudy.top

================================================================================
来源：http://tky.chenlongwang.top

[G01] 定义类
来源：http://hgh.zdbjq.cn


<!-- 参考信息 -->