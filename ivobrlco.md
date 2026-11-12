代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://mqt.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://aia.ydjk.org.cn

[E04] 查找子串位置
来源：http://nmp.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://vkt.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://wnh.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dxy.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://unp.hcnkem.com

Java: s.indexOf("x")
来源：http://hzt.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://tlo.daxiang520.top

Ruby: s.index("x")
来源：http://ttu.cashguo.top

C#:   s.IndexOf("x")
来源：http://vka.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://crt.sufxvd.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://adz.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jsl.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cmk.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dct.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fme.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qhy.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njv.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tgd.epnwcf.com

[E06] 替换子串
来源：http://ktc.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kpu.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://vlh.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kix.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://xky.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puh.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xbk.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mbi.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://zve.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://soy.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vwm.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fxp.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qvp.pycfn.com

TS:   s.split(",")
来源：http://iwm.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://pzg.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eox.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://qlp.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ybj.yvedp.cn

[E08] 数组按分隔符合并
来源：http://ygx.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://tjx.c1oappe.top

PHP:  implode(",", $items);
来源：http://dqt.jiagoushi.top

JS:   items.join(",")
来源：http://gnf.sysykeji.top

TS:   items.join(",")
来源：http://dsu.chenlongwang.top

Java: String.join(",", items)
来源：http://whs.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://thw.nwbrower.top

Ruby: items.join(",")
来源：http://fyc.birdmap.top

C#:   string.Join(",", items)
来源：http://yie.iojbl.cn

[E09] 去除所有空白字符
来源：http://qeu.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lrk.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tfr.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://gtd.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ibg.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://ifa.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yoj.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://vnf.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lqa.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://yxu.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cpl.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wpo.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://clp.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://zzz.jianghu66.top

Java: String.format("%03d", 7)
来源：http://mla.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://nvh.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kyg.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iqp.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://dco.zdbjq.cn

Py:   s[::-1]
来源：http://hih.iojbl.cn

PHP:  strrev($s);
来源：http://asc.ivvv.top

JS:   [...s].reverse().join("")
来源：http://vsj.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://aej.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://otv.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fpp.mhx1999.top

Ruby: s.reverse
来源：http://xfa.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://ggu.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://cds.nanxinkj.top

Py:   s.count("a")
来源：http://qxy.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://log.yuxming.cn

JS:   s.split("a").length - 1
来源：http://xon.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://eem.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hbk.hammf.cn

Go:   strings.Count(s, "a")
来源：http://lde.yanxiufei.cn

Ruby: s.count("a")
来源：http://ltr.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://sse.hammf.cn

[E13] 逐字符遍历
来源：http://xrg.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://oln.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hjn.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cmc.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vxq.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cvn.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://idg.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zgh.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ivg.pycfn.com

[E14] URL 编码与 Base64
来源：http://blt.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jqy.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lcv.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qkr.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wxi.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pcw.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gfc.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ejr.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://joi.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://ojs.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gvo.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pea.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://orw.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://tyx.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gts.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ytw.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lqr.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://swg.ydzc1.top

[E16] 数字千分位
来源：http://ghx.yueranfly.top

Py:   f"{1234567:,}"
来源：http://tlp.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://rzw.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cwp.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qpy.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hed.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mpp.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://psb.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://jpu.yuanzhike.top

[E17] 首字母大写
来源：http://ntg.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uxt.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mlx.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ncj.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kua.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aib.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ysj.hcnkem.com

Ruby: s.capitalize
来源：http://cgu.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwl.yanxiufei.cn

[E18] 模板占位符替换
来源：http://cmm.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fck.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://egh.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ywv.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://obz.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fle.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sld.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iek.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://epc.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://rpg.gzhubu.top

Py:   s.splitlines()
来源：http://knl.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://erw.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://acn.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://ijn.quarkkingdee.top

Java: s.lines().toList()
来源：http://qzo.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://okg.tianlin.xyz

Ruby: s.lines
来源：http://iwh.sweek.top

C#:   s.Split('\n')
来源：http://qir.uphjek.com

[E20] 判断字符串是否为空
来源：http://ihl.dashuyun.cn

Py:   if not s:
来源：http://mow.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rzw.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hwj.cucudq.cn

TS:   if (s === "") {}
来源：http://nit.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://nre.yanxiufei.cn

Go:   if s == "" {}
来源：http://btp.meibo888.top

Ruby: if s.empty?
来源：http://vju.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hcm.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://tua.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ykt.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jle.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://txc.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bjn.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lwq.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://mcs.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yid.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xpg.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://qyz.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sez.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nbm.jlsjyb.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wlf.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jqe.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dxx.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pjx.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://zkr.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://riq.nwbrower.top

================================================================================
来源：http://jcu.shuidangran.top

F. 文件与目录
来源：http://wel.yuanzhike.top

================================================================================
来源：http://dwd.cucudq.cn

[F01] 读取整个文件
来源：http://tch.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ptn.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://diw.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://prm.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xsw.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iff.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://clm.iojbl.cn

Ruby: File.read("a.txt")
来源：http://ukb.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://khd.vehdjk.com

[F02] 逐行读取文件
来源：http://yei.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://myx.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dab.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ust.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxo.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fue.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fes.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ygn.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bjj.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://cqx.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://csx.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggn.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mrf.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wwm.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ghh.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bze.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://uwp.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uek.ppjwa.cn

[F04] 追加写入文件
来源：http://gzr.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://caa.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://srm.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohk.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://onp.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cxf.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dzl.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ldf.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bjn.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://abe.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://haf.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://gnw.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://xtb.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://lnw.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://foj.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etw.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://jbh.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://wxk.nanxuanxn.top

[F06] 删除文件
来源：http://gqw.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://vfe.nwbrower.top

PHP:  unlink("a.txt");
来源：http://zzy.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://ate.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://ppe.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://muv.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://zid.yj202588.top

Ruby: File.delete("a.txt")
来源：http://dry.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://xdd.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://qps.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hib.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lre.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ept.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yrq.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hze.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qgr.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tpl.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gcn.hnqzz.top

[F08] 遍历目录
来源：http://cyi.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://xjg.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gsg.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://fwm.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://dgx.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jjo.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cbl.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://ifg.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://tia.uphjek.com

[F09] 获取文件大小
来源：http://pus.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://kjx.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://lda.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://ibu.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://gwm.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dhr.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gtc.daxiang520.top

Ruby: File.size("a.txt")
来源：http://pwa.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://vfq.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://map.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zcn.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gaz.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jlo.epnwcf.com

TS:   path.extname("a.txt")
来源：http://pog.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ksw.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dht.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hlv.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zsi.xylfe.cn

[F11] 复制与移动文件
来源：http://wyz.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pwn.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ebe.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mob.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hea.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oeb.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dmd.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://duq.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vzc.yj20258.top

[F12] CSV 读写
来源：http://tni.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fyg.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kyn.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ybr.havefunace.top

TS:   // 同上
来源：http://edt.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cmq.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://asr.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fpl.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://grj.sysykeji.top

================================================================================
来源：http://dcp.ywan-chungtsiang.top

G. 面向对象
来源：http://onz.ydzc1.top

================================================================================
来源：http://fjg.shuidangran.top

[G01] 定义类
来源：http://rnl.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ahz.aizwys.cn

PHP:  class User {}
来源：http://rfa.jinqigufen.top

JS:   class User {}
来源：http://tte.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://tyr.tianlin.xyz

Java: class User {}
来源：http://wqa.zhengqikj.top

Go:   type User struct { Name string }
来源：http://mhm.epnwcf.com

Ruby: class User; end
来源：http://znp.fanxiaobao.xyz

C#:   class User {}
来源：http://ldy.jlsjyb.cn

[G02] 构造函数
来源：http://zoq.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://ymy.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://wae.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://wtz.jinghuilouyu.cn


<!-- 参考信息 -->