代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ygt.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://yjx.hammf.cn

Java: s.substring(1, 4)
来源：http://ygf.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://izl.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://voi.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://wav.hcnkem.com

[E04] 查找子串位置
来源：http://zgu.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://mib.vehdjk.com

PHP:  strpos($s, "x");
来源：http://gjt.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://clw.jqgfzy.top

TS:   s.indexOf("x")
来源：http://tfs.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://hoy.tanke756.top

Go:   strings.Index(s, "x")
来源：http://jdt.jyoumei.cn

Ruby: s.index("x")
来源：http://udx.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://upj.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uhy.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://act.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tcp.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avw.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ios.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zfk.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yto.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mdo.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nsi.guowangkeji.top

[E06] 替换子串
来源：http://ztw.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mvi.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://ims.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vco.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://req.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oto.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xza.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ykp.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://xci.yonumen.top

[E07] 按分隔符拆分
来源：http://oky.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xwo.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zau.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mtu.zhiwuduotai.top

TS:   s.split(",")
来源：http://bzy.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mpz.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zss.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://imz.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ucn.yueranfly.top

[E08] 数组按分隔符合并
来源：http://ade.yanxiufei.cn

Py:   ",".join(items)
来源：http://ttn.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://cyz.tianlin.xyz

JS:   items.join(",")
来源：http://ogi.nwbrower.top

TS:   items.join(",")
来源：http://lao.cqqwz.cn

Java: String.join(",", items)
来源：http://mzo.ivvv.top

Go:   strings.Join(items, ",")
来源：http://ayz.yongpay.top

Ruby: items.join(",")
来源：http://qbs.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://ucx.ivvv.top

[E09] 去除所有空白字符
来源：http://ygl.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://clj.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rks.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://sxl.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://jxz.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://lwz.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://asn.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://xvv.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jlm.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://ytm.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hpq.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zcw.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://kvt.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://rdz.bbcook.cn

Java: String.format("%03d", 7)
来源：http://ajq.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aur.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://adp.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ipz.meibo888.top

[E11] 反转字符串
来源：http://mdt.mhx1999.top

Py:   s[::-1]
来源：http://kmp.andypj.xyz

PHP:  strrev($s);
来源：http://glb.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://uqi.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://nzm.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fth.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wde.yj20258888.top

Ruby: s.reverse
来源：http://ajz.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://mcs.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://jug.yfazqb.com

Py:   s.count("a")
来源：http://jgj.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://kto.yfazqb.com

JS:   s.split("a").length - 1
来源：http://hyk.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://lyo.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://onl.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://fht.tarul.cn

Ruby: s.count("a")
来源：http://zrw.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://ain.cashguo.top

[E13] 逐字符遍历
来源：http://wit.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://vgt.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://trw.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xzz.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qre.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bsb.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://luo.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://xfe.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zjk.daria6918.cn

[E14] URL 编码与 Base64
来源：http://zqi.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ysd.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ijr.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ozz.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fvq.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iho.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://amv.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vqw.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://onk.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://fqy.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://plp.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zjg.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gpx.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sni.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kcn.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fvm.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sjd.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://psw.0kj1m.cn

[E16] 数字千分位
来源：http://syn.pycfn.com

Py:   f"{1234567:,}"
来源：http://tof.hysaishi.cn

PHP:  number_format(1234567);
来源：http://kzg.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fph.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aya.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mkm.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kqc.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vak.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://dsm.meibo888.top

[E17] 首字母大写
来源：http://oxm.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hdg.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fcg.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fsd.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iof.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxp.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yqb.jinqigufen.top

Ruby: s.capitalize
来源：http://bkr.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qlr.iojbl.cn

[E18] 模板占位符替换
来源：http://twx.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://krv.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xqw.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bks.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://gnx.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bsi.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://flr.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uxc.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zwl.yuxming.cn

[E19] 多行文本按行拆分
来源：http://hzu.shuidangran.top

Py:   s.splitlines()
来源：http://dim.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nyk.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://awo.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://nbx.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://tdr.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://vjq.yueranfly.top

Ruby: s.lines
来源：http://gzj.bjfxy.top

C#:   s.Split('\n')
来源：http://jhe.316326.xyz

[E20] 判断字符串是否为空
来源：http://thi.sysykeji.top

Py:   if not s:
来源：http://juq.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jdr.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zed.meibo888.top

TS:   if (s === "") {}
来源：http://lpd.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://prk.yongpay.top

Go:   if s == "" {}
来源：http://fbt.gaohongyu789.top

Ruby: if s.empty?
来源：http://dza.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xel.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://nhu.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://olg.hnxiangtu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rfy.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vic.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vtu.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://imo.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://bss.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gsy.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qkp.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://mqk.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qny.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kxe.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rit.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gfa.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rll.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gwg.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://vaf.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lnn.ybcxt.top

================================================================================
来源：http://mjo.ctjpmb.com

F. 文件与目录
来源：http://afk.hfpthk.cn

================================================================================
来源：http://vax.smart0.xyz

[F01] 读取整个文件
来源：http://gvx.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yuc.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://pam.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pnb.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fjx.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cow.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ssu.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://egw.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://pah.pycfn.com

[F02] 逐行读取文件
来源：http://ugr.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kjv.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pzi.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dnt.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iea.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://znh.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://upa.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rzf.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://afe.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://tpj.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kzc.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gly.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://srp.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://suc.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rlx.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ljl.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://fvx.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vyo.tian-w.cn

[F04] 追加写入文件
来源：http://tnx.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qpq.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://myh.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ouy.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kcl.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pyf.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ifa.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ybg.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bnf.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://rcf.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pcb.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://jtt.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://win.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://gyz.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://myv.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qvg.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://pga.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://egg.epnwcf.com

[F06] 删除文件
来源：http://aas.sxryk.cn

Py:   os.remove("a.txt")
来源：http://nko.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://ycj.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://lhx.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://fbr.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://osl.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://cjg.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://oom.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://ahg.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://avf.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gcv.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fst.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eqt.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wec.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cwf.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lvq.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://esa.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ddn.quarkkingdee.top

[F08] 遍历目录
来源：http://inx.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://njb.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tum.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://eci.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://rgz.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://etg.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xas.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://txm.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://kqm.yanxiufei.cn

[F09] 获取文件大小
来源：http://eel.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://unp.gzhubu.top

PHP:  filesize("a.txt");
来源：http://ojz.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://iqn.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://eat.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://hcc.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wwe.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://fmx.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://rhi.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://xtv.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yym.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gqw.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hrq.shuidangran.top

TS:   path.extname("a.txt")
来源：http://cqf.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ukb.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pju.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mzl.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ajq.jqgfzy.top

[F11] 复制与移动文件
来源：http://ade.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eip.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baq.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fde.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://slc.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ecw.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pim.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://syy.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aen.kuanghao11.cn

[F12] CSV 读写
来源：http://wlu.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sxo.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zjl.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uan.sjlbkw.cn

TS:   // 同上
来源：http://mpr.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uks.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://whs.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tim.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://iag.nwbrower.top

================================================================================
来源：http://otp.ctjpmb.com

G. 面向对象
来源：http://hfw.feifeiyinyue.top

================================================================================
来源：http://ozm.uphjek.com

[G01] 定义类
来源：http://adr.jinqigufen.top

Py:   class User: pass
来源：http://lcs.yj20258.top

PHP:  class User {}
来源：http://bzd.zhaomingkeji.xyz

JS:   class User {}
来源：http://lmj.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://iae.shzxlz.cn

Java: class User {}
来源：http://uds.zhengqikj.top

Go:   type User struct { Name string }
来源：http://xel.meibo888.top

Ruby: class User; end
来源：http://ysk.c1oappe.top

C#:   class User {}
来源：http://ybu.jinghuilouyu.cn


<!-- 参考信息 -->