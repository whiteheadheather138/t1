代发 wailian999

PHP:  strpos($s, "x");
来源：http://dyc.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fle.vehdjk.com

TS:   s.indexOf("x")
来源：http://fyl.tian-w.cn

Java: s.indexOf("x")
来源：http://zos.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://fdx.xylfe.cn

Ruby: s.index("x")
来源：http://zmv.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://pqm.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rdh.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ppm.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://snp.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xsu.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://gjz.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hkk.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://djs.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://apx.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eds.gogol.net.cn

[E06] 替换子串
来源：http://rrl.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://flo.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://ubx.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqa.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://ekq.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yhr.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hsv.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wpc.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://ura.yueranfly.top

[E07] 按分隔符拆分
来源：http://bsp.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mdi.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nbg.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://otd.hammf.cn

TS:   s.split(",")
来源：http://vsj.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://mfe.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jvg.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://pvz.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dor.wangdashe.top

[E08] 数组按分隔符合并
来源：http://qnt.kuanghao11.cn

Py:   ",".join(items)
来源：http://qfq.cdnleiting.top

PHP:  implode(",", $items);
来源：http://urc.xylfe.cn

JS:   items.join(",")
来源：http://cwv.tianlin.xyz

TS:   items.join(",")
来源：http://zgh.cdnleiting.top

Java: String.join(",", items)
来源：http://cca.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://fwg.yangfankeji.com

Ruby: items.join(",")
来源：http://uir.hnqzz.top

C#:   string.Join(",", items)
来源：http://nrj.yuxming.cn

[E09] 去除所有空白字符
来源：http://gzo.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wis.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kem.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://bfu.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://qol.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://paj.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://plc.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://iev.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eyy.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://eql.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sqn.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wmh.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://arr.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://cac.meibo888.top

Java: String.format("%03d", 7)
来源：http://smk.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://buc.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ebf.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ujn.jlsjyb.cn

[E11] 反转字符串
来源：http://hnz.feifeiyinyue.top

Py:   s[::-1]
来源：http://lno.pengpengdd.cyou

PHP:  strrev($s);
来源：http://afv.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://vho.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://urx.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cqz.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ssi.cdnleiting.top

Ruby: s.reverse
来源：http://zrq.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://lny.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://aix.c1oappe.top

Py:   s.count("a")
来源：http://npa.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://yjr.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://rsh.nwbrower.top

TS:   s.split("a").length - 1
来源：http://oip.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qfe.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://vos.hcnkem.com

Ruby: s.count("a")
来源：http://xhi.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://cci.shzxlz.cn

[E13] 逐字符遍历
来源：http://tsz.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://yto.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gti.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://spx.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://awe.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eoe.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gjt.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://gae.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ioo.uphjek.com

[E14] URL 编码与 Base64
来源：http://qzs.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tjo.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gmy.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://igv.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rfi.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zbm.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zka.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nvz.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bxc.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://xdh.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://zoc.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://icr.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pxz.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kgi.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dba.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zua.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cud.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sjf.quarkkingdee.top

[E16] 数字千分位
来源：http://sav.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://oea.mhx1999.top

PHP:  number_format(1234567);
来源：http://otp.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ydq.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://erh.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tbu.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://csd.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://svh.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://dwx.nwbrower.top

[E17] 首字母大写
来源：http://xly.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jiv.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://deu.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljl.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vyy.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dsb.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fvs.tarul.cn

Ruby: s.capitalize
来源：http://lub.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tuj.52xcode.cn

[E18] 模板占位符替换
来源：http://ctr.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jis.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tij.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zqs.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xmn.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pde.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tvl.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uyq.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pvc.sweek.top

[E19] 多行文本按行拆分
来源：http://cdi.sjlbkw.cn

Py:   s.splitlines()
来源：http://zql.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rae.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://ohf.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://cfb.nanxinkj.top

Java: s.lines().toList()
来源：http://ucv.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://nnl.ivvv.top

Ruby: s.lines
来源：http://zpz.haohaochexian.top

C#:   s.Split('\n')
来源：http://mmn.yj202588.top

[E20] 判断字符串是否为空
来源：http://bru.cheryme.top

Py:   if not s:
来源：http://tyl.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jfg.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fbg.fzhhl.top

TS:   if (s === "") {}
来源：http://mvu.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://mvt.jiagoushi.top

Go:   if s == "" {}
来源：http://cda.uphjek.com

Ruby: if s.empty?
来源：http://lpb.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://apw.pycfn.com

[E21] 超长截断加省略号
来源：http://wkc.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oqr.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ljc.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://spf.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iyl.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bgm.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://muz.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rei.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lsp.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://gqy.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://unp.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osf.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://thy.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cat.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wsr.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kcg.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://wba.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://erj.9152youxi.cn

================================================================================
来源：http://ycu.kuanghao11.cn

F. 文件与目录
来源：http://ehx.hywenlv.cn

================================================================================
来源：http://rot.yfazqb.com

[F01] 读取整个文件
来源：http://ykt.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gla.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://fhv.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jop.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wdw.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://pjd.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fod.yfazqb.com

Ruby: File.read("a.txt")
来源：http://vzd.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://pas.redwolf501.top

[F02] 逐行读取文件
来源：http://qjx.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://azs.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjj.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nlm.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swc.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://atd.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mjd.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fqc.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zkn.tanke756.top

[F03] 写入文件（覆盖）
来源：http://zns.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ngf.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ijl.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hob.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gbl.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zxm.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jvr.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://ygn.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cxz.ehwqpu.com

[F04] 追加写入文件
来源：http://gdi.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://obv.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vsv.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbc.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://otj.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yuq.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://boq.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yzj.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nzn.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://qqo.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nfp.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://njl.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://ujz.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://xjg.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rnk.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etp.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://crf.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://lsx.birdmap.top

[F06] 删除文件
来源：http://axz.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://jgi.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://irc.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://lxc.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://pcg.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hym.pycfn.com

Go:   os.Remove("a.txt")
来源：http://smm.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://oyf.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://osj.xuanzx.com

[F07] 创建目录（含多级）
来源：http://rle.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oem.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://elw.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://txm.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://itp.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lvy.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://biu.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kli.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mnc.daxiang520.top

[F08] 遍历目录
来源：http://xxz.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tzk.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://isv.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://ruc.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://oez.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mez.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://crs.yj20258888.top

Ruby: Dir.children("dir")
来源：http://wtk.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://xga.yueranfly.top

[F09] 获取文件大小
来源：http://zdy.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://dkp.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://jti.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://suv.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://sed.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bqy.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tpw.fengsongda.top

Ruby: File.size("a.txt")
来源：http://ocn.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://erj.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://ldn.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lnj.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lcg.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tqf.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://jlc.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jnl.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mmg.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ftc.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ngi.epnwcf.com

[F11] 复制与移动文件
来源：http://tda.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rxm.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ygs.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xmj.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fye.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rln.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tfr.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dcp.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hmt.wangshuangyany.cn

[F12] CSV 读写
来源：http://jyk.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://arj.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cxs.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zgf.jinghuilouyu.cn

TS:   // 同上
来源：http://pqg.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bjv.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eqt.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zsc.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://otp.chenjidiqi.icu

================================================================================
来源：http://btw.xingfuxueyuan.xyz

G. 面向对象
来源：http://raf.ydjk.org.cn

================================================================================
来源：http://vtg.quarkkingdee.top

[G01] 定义类
来源：http://jlr.vehdjk.com

Py:   class User: pass
来源：http://buo.xziqi.cn

PHP:  class User {}
来源：http://hrm.0kj1m.cn

JS:   class User {}
来源：http://vif.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://jcj.cucudq.cn

Java: class User {}
来源：http://svp.snrcjt.cn

Go:   type User struct { Name string }
来源：http://ixe.sxryk.cn

Ruby: class User; end
来源：http://exw.fzhhl.top

C#:   class User {}
来源：http://keo.pycfn.com

[G02] 构造函数
来源：http://ath.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://inl.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://ksz.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://gdx.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://pcj.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://fij.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mva.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://hzj.shanyushiyangtech.top


<!-- 参考信息 -->