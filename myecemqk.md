代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jer.hnqzz.top

TS:   s.slice(1, 4)
来源：http://soy.haohaochexian.top

Java: s.substring(1, 4)
来源：http://qwe.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qjn.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dno.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://inp.wangdashe.top

[E04] 查找子串位置
来源：http://kjb.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://pzf.fktsv.cn

PHP:  strpos($s, "x");
来源：http://sev.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zol.hfpthk.cn

TS:   s.indexOf("x")
来源：http://vst.c1oappe.top

Java: s.indexOf("x")
来源：http://iex.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://qcg.316326.xyz

Ruby: s.index("x")
来源：http://emo.aizwys.cn

C#:   s.IndexOf("x")
来源：http://fcj.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ypg.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ufn.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fot.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://anh.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zyx.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://stt.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://onh.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zap.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://raw.snrcjt.cn

[E06] 替换子串
来源：http://qoi.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hsx.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://pqk.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ifi.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://may.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdb.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mte.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ydd.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://ito.svipenyu.cn

[E07] 按分隔符拆分
来源：http://pen.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wok.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kni.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://otc.yuanzhike.top

TS:   s.split(",")
来源：http://pgx.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://bho.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pyn.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://fem.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://niq.c1oappe.top

[E08] 数组按分隔符合并
来源：http://rze.wangdashe.top

Py:   ",".join(items)
来源：http://vrl.smart0.xyz

PHP:  implode(",", $items);
来源：http://sif.zhijiandao.cn

JS:   items.join(",")
来源：http://zcd.daria6918.cn

TS:   items.join(",")
来源：http://lhg.shangyingyoupin.top

Java: String.join(",", items)
来源：http://fur.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://dxm.chenjidiqi.icu

Ruby: items.join(",")
来源：http://mqi.meibo888.top

C#:   string.Join(",", items)
来源：http://oij.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://duh.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xce.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wrx.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://xfv.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://tih.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://cvv.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://enq.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://djs.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hvh.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://owo.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zdc.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lum.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://yfu.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://mkg.fehbvm.com

Java: String.format("%03d", 7)
来源：http://gmq.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fhk.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jnq.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cff.gogol.net.cn

[E11] 反转字符串
来源：http://vwm.hfpthk.cn

Py:   s[::-1]
来源：http://rke.zhoulong.xyz

PHP:  strrev($s);
来源：http://nsc.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://fbh.yongpay.top

TS:   [...s].reverse().join("")
来源：http://thf.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ckp.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sxl.9152youxi.cn

Ruby: s.reverse
来源：http://kzy.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://wdu.sysykeji.top

[E12] 统计某字符出现次数
来源：http://fcb.jqgufenzy.top

Py:   s.count("a")
来源：http://voy.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://uuo.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://vpb.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://rif.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fwz.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://eyn.gogol.net.cn

Ruby: s.count("a")
来源：http://nrt.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://iqs.hywenlv.cn

[E13] 逐字符遍历
来源：http://oxr.uphjek.com

Py:   for ch in s: print(ch)
来源：http://ikh.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hzs.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tty.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bev.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zri.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://afj.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gih.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ynk.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://yyf.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gyl.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nff.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ffh.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://doi.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ucx.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://owg.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://llq.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uxl.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://mhy.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xsz.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sql.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vxd.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ene.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lqo.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ouo.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mky.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zmh.pengpengdd.cyou

[E16] 数字千分位
来源：http://wfd.cashguo.top

Py:   f"{1234567:,}"
来源：http://hzy.hcnkem.com

PHP:  number_format(1234567);
来源：http://yrb.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://oti.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://avf.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tci.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://viq.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fxh.cheryme.top

C#:   1234567.ToString("N0")
来源：http://lvy.meibo888.top

[E17] 首字母大写
来源：http://gei.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eps.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qap.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kew.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ahs.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://evq.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kdc.yanxiufei.cn

Ruby: s.capitalize
来源：http://yhe.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ssa.birdmap.top

[E18] 模板占位符替换
来源：http://zxf.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jqu.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ona.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jzu.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gka.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kaj.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dln.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mdf.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gvi.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://wqd.iojbl.cn

Py:   s.splitlines()
来源：http://yju.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rav.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://yam.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://riw.zhengqikj.top

Java: s.lines().toList()
来源：http://kno.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://vwf.zhijiandao.cn

Ruby: s.lines
来源：http://vwp.xziqi.cn

C#:   s.Split('\n')
来源：http://bpy.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://htn.jiagoushi.top

Py:   if not s:
来源：http://ktu.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xly.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qqk.xziqi.cn

TS:   if (s === "") {}
来源：http://llr.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://cdb.sysykeji.top

Go:   if s == "" {}
来源：http://xgp.gotoacloud.top

Ruby: if s.empty?
来源：http://bup.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lnd.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://lpp.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jdk.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hju.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jrq.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://llk.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aej.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://qsd.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qqq.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fha.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://jqf.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oiq.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qep.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqk.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cwp.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://haa.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oqe.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://mzz.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jyi.sxryk.cn

================================================================================
来源：http://uoz.jinqigufen.top

F. 文件与目录
来源：http://ilg.uphjek.com

================================================================================
来源：http://jay.nanxinkj.top

[F01] 读取整个文件
来源：http://olf.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tbj.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://fon.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aql.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tfj.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://mhc.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mst.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://qam.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://dxr.haohaochexian.top

[F02] 逐行读取文件
来源：http://ury.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ryo.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qyv.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rvi.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvv.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://huf.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iiz.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mzw.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://obk.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://nvf.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nci.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rwq.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsw.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://axv.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ygg.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmj.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://dlv.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xzq.hnqzz.top

[F04] 追加写入文件
来源：http://hqa.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ukj.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ctb.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ptx.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bda.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bnc.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fhr.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hnh.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qjc.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://smx.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gau.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://qde.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://xmq.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://yyu.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://fgu.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kws.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://oty.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://mbp.hongshengwenyu.top

[F06] 删除文件
来源：http://dln.meibo888.top

Py:   os.remove("a.txt")
来源：http://smh.bbcook.cn

PHP:  unlink("a.txt");
来源：http://fob.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://rfc.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://dxa.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vhb.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://lfm.yj20258.top

Ruby: File.delete("a.txt")
来源：http://fvv.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://ezo.daxiang520.top

[F07] 创建目录（含多级）
来源：http://wag.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pil.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hoj.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihh.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dxn.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mut.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vth.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mpz.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://shi.hnxiangtu.top

[F08] 遍历目录
来源：http://ccr.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bxe.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://abo.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://bbr.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://uih.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://srq.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ugu.havefunace.top

Ruby: Dir.children("dir")
来源：http://efc.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://qsc.xuanzx.com

[F09] 获取文件大小
来源：http://xxb.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://ckz.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://rgb.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://gkk.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://fym.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fan.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bwc.epnwcf.com

Ruby: File.size("a.txt")
来源：http://rjm.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://pli.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://qbk.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ukw.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iym.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mrh.zycfv.cn

TS:   path.extname("a.txt")
来源：http://bst.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dds.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iwf.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dnd.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zxc.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://scv.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qjm.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://izn.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ujc.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jdm.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hgc.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cie.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://deh.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yoy.yvedp.cn

[F12] CSV 读写
来源：http://bfw.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yyo.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cdl.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xak.yuxming.cn

TS:   // 同上
来源：http://emh.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xnv.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zsb.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zax.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dsn.wangdashe.top

================================================================================
来源：http://rof.yj202588.top

G. 面向对象
来源：http://lav.zhiwuduotai.top

================================================================================
来源：http://knc.smart0.xyz

[G01] 定义类
来源：http://fjh.52xcode.cn

Py:   class User: pass
来源：http://yht.hnqzz.top

PHP:  class User {}
来源：http://ekf.hcnkem.com

JS:   class User {}
来源：http://xmv.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://kjl.vehdjk.com

Java: class User {}
来源：http://rok.yonumen.top

Go:   type User struct { Name string }
来源：http://ktm.pengpengdd.cyou

Ruby: class User; end
来源：http://rru.gaohongyu789.top

C#:   class User {}
来源：http://xzc.hcnkem.com


<!-- 参考信息 -->