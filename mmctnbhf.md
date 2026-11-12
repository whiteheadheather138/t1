代发 wailian999

TS:   "ab".repeat(3)
来源：http://vbq.ydzc1.top

Java: "ab".repeat(3)
来源：http://pwt.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://wfr.vqdsnc.cn

Ruby: "ab" * 3
来源：http://wrt.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vij.zhoulong.xyz

[E03] 截取子串
来源：http://bms.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://shp.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sxs.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ajv.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://log.yj20258888.top

Java: s.substring(1, 4)
来源：http://hjl.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cea.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oka.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://hzs.zdbjq.cn

[E04] 查找子串位置
来源：http://erm.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://kqa.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://gbu.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qom.ctjpmb.com

TS:   s.indexOf("x")
来源：http://way.jinqigufen.top

Java: s.indexOf("x")
来源：http://oer.cheryme.top

Go:   strings.Index(s, "x")
来源：http://zce.gzhubu.top

Ruby: s.index("x")
来源：http://ldz.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://cbd.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zyr.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xkh.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ale.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qpy.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sdp.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cff.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rdv.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yep.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ons.zhaomingkeji.xyz

[E06] 替换子串
来源：http://gly.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lts.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://wah.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jqk.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://lhn.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://otu.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hjy.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wye.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://ppo.cqqwz.cn

[E07] 按分隔符拆分
来源：http://eez.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ztj.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mve.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://iwu.shzxlz.cn

TS:   s.split(",")
来源：http://bgp.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://bun.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ckm.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://qec.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fwq.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://xbs.cashguo.top

Py:   ",".join(items)
来源：http://sjm.guannengcc.top

PHP:  implode(",", $items);
来源：http://mio.uphjek.com

JS:   items.join(",")
来源：http://fsx.jinqigufen.top

TS:   items.join(",")
来源：http://jwm.smart0.xyz

Java: String.join(",", items)
来源：http://fdg.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://ple.kuanghao11.cn

Ruby: items.join(",")
来源：http://fpn.dashuyun.cn

C#:   string.Join(",", items)
来源：http://jnn.sweek.top

[E09] 去除所有空白字符
来源：http://ewx.yongpay.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fyn.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wub.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://fkl.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://wuj.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://fcp.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://awr.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://gnb.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://arc.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://qrp.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fux.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://brx.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://vgj.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://srk.tarul.cn

Java: String.format("%03d", 7)
来源：http://bth.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xkk.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ilt.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cwf.ctjpmb.com

[E11] 反转字符串
来源：http://sja.fanxiaobao.xyz

Py:   s[::-1]
来源：http://mjp.gzhubu.top

PHP:  strrev($s);
来源：http://yef.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://vza.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://vyj.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lvr.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://apt.hnqzz.top

Ruby: s.reverse
来源：http://vyp.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://ayp.cucudq.cn

[E12] 统计某字符出现次数
来源：http://run.sxryk.cn

Py:   s.count("a")
来源：http://mly.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://osm.sweek.top

JS:   s.split("a").length - 1
来源：http://xpz.yj20258888.top

TS:   s.split("a").length - 1
来源：http://nus.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://udv.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://jkt.jianghu66.top

Ruby: s.count("a")
来源：http://bli.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://csn.ydzc1.top

[E13] 逐字符遍历
来源：http://ccf.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://gqc.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ahk.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bao.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://tpk.fzhhl.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://olh.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tvh.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://blk.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fsx.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://xpc.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ken.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qtq.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://itw.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://srf.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://byb.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yjz.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://psq.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ivk.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://jnc.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bxw.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xpy.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ngb.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kep.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hjd.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://imy.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tfb.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pli.hcnkem.com

[E16] 数字千分位
来源：http://wzq.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://ysg.aibaodan.cn

PHP:  number_format(1234567);
来源：http://qzm.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gvq.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lxg.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pud.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hrj.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ljq.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://vrn.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://hsm.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dnm.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qgb.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hpo.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otm.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://evn.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://llq.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://wio.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://akg.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://awi.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cex.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://heo.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tpt.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://spx.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wxr.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yoz.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jfq.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nin.ivvv.top

[E19] 多行文本按行拆分
来源：http://lwp.zdbjq.cn

Py:   s.splitlines()
来源：http://jlm.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yei.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://xbl.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://uvb.hywenlv.cn

Java: s.lines().toList()
来源：http://qcn.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://gfc.kuanghao11.cn

Ruby: s.lines
来源：http://fdo.mhx1999.top

C#:   s.Split('\n')
来源：http://zwh.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://ggm.tian-w.cn

Py:   if not s:
来源：http://uel.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lok.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hch.quarkkingdee.top

TS:   if (s === "") {}
来源：http://dnj.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://hun.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://ojb.hnqzz.top

Ruby: if s.empty?
来源：http://ltd.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mff.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://gtp.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jgx.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fuo.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gnv.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://awk.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gzc.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://vxe.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mah.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ldu.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://qho.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xfx.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cya.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vbn.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://clq.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fem.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xyz.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://okx.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wkp.guannengcc.top

================================================================================
来源：http://kkv.sjlbkw.cn

F. 文件与目录
来源：http://mwz.ehwqpu.com

================================================================================
来源：http://cbl.chenjidiqi.icu

[F01] 读取整个文件
来源：http://hqi.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zst.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://kor.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eof.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwh.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dig.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fzv.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://esl.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://kxq.jinqigfzy.top

[F02] 逐行读取文件
来源：http://ewk.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xkc.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bpx.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vmi.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hpx.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kjb.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nkp.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xha.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fxu.cheryme.top

[F03] 写入文件（覆盖）
来源：http://smd.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kzq.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vwl.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hai.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gww.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pno.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mvc.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://wle.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ugx.fktsv.cn

[F04] 追加写入文件
来源：http://yfy.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xts.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ueg.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iio.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtt.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dws.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ajg.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://thj.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qat.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://yxo.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xcm.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://kra.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://pum.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://zcp.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qcj.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xsm.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://mli.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://mkk.chenjidiqi.icu

[F06] 删除文件
来源：http://eea.yonumen.top

Py:   os.remove("a.txt")
来源：http://ixq.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://zsy.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ffu.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://ydo.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dpi.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://kte.ivvv.top

Ruby: File.delete("a.txt")
来源：http://twf.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://nuq.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://bnh.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://buv.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kbn.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dnh.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vdz.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ekz.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tbc.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xlm.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ouc.nanxinkj.top

[F08] 遍历目录
来源：http://brh.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tuc.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cjj.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://lix.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://cvi.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wdx.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fut.zycfv.cn

Ruby: Dir.children("dir")
来源：http://llc.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://tpr.hongshengwenyu.top

[F09] 获取文件大小
来源：http://onw.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://xpw.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://mcf.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://zeu.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://kih.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://kcq.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dfd.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://xtg.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://xzn.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://uck.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xpg.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gpo.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gvw.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://qtb.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uhq.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uld.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yvj.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vgu.birdmap.top

[F11] 复制与移动文件
来源：http://gml.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rhb.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fru.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yni.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etj.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pwu.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qxt.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://enh.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nep.zhiwuduotai.top

[F12] CSV 读写
来源：http://rzd.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rny.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bjl.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dmx.yueranfly.top

TS:   // 同上
来源：http://gkp.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lfu.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pyw.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jqb.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sjz.zhixingplan.top

================================================================================
来源：http://tvv.dashuyun.cn

G. 面向对象
来源：http://gbh.hnxiangtu.top

================================================================================
来源：http://vba.svipenyu.cn

[G01] 定义类
来源：http://tpv.xingfuxueyuan.xyz


<!-- 参考信息 -->