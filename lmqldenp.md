代发 wailian999

PHP:  strpos($s, "x");
来源：http://dna.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jfg.cqqwz.cn

TS:   s.indexOf("x")
来源：http://dui.ivvv.top

Java: s.indexOf("x")
来源：http://wzc.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://xur.redwolf501.top

Ruby: s.index("x")
来源：http://eua.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://xmm.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mbk.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dpv.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://way.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tup.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://nxc.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://awq.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hio.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pww.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fsp.haohaochexian.top

[E06] 替换子串
来源：http://kfg.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://row.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://jbt.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pqq.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://ojq.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vtg.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cih.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://npj.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://wlg.xylfe.cn

[E07] 按分隔符拆分
来源：http://trv.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kpj.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fez.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://onl.yanxiufei.cn

TS:   s.split(",")
来源：http://xac.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xdw.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://orn.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://djl.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://epx.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://hkv.yanxiufei.cn

Py:   ",".join(items)
来源：http://ajo.chenzaomai.com

PHP:  implode(",", $items);
来源：http://fqm.zhoulong.xyz

JS:   items.join(",")
来源：http://nae.vehdjk.com

TS:   items.join(",")
来源：http://vbw.ppjwa.cn

Java: String.join(",", items)
来源：http://efx.316326.xyz

Go:   strings.Join(items, ",")
来源：http://dzl.nwbrower.top

Ruby: items.join(",")
来源：http://iwn.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://ujm.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://qgz.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zjs.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wrj.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://ivw.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://stl.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xex.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tuw.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://osr.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yfb.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://pyy.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dje.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://afq.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://mlh.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://gii.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://qfe.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zsv.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eyl.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dmk.jinghuilouyu.cn

[E11] 反转字符串
来源：http://byn.meibo888.top

Py:   s[::-1]
来源：http://sfk.hnqzz.top

PHP:  strrev($s);
来源：http://xhv.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://alz.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://foy.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jey.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xtb.daria6918.cn

Ruby: s.reverse
来源：http://gre.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://xba.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://fbs.sjlbkw.cn

Py:   s.count("a")
来源：http://uei.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://xju.hcnkem.com

JS:   s.split("a").length - 1
来源：http://tls.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://eyh.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bzl.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://tgt.vehdjk.com

Ruby: s.count("a")
来源：http://ypo.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://oiy.xuanzx.com

[E13] 逐字符遍历
来源：http://qcy.birdmap.top

Py:   for ch in s: print(ch)
来源：http://mki.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vte.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eno.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vqi.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pla.gzhubu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://krd.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ydw.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rod.andypj.xyz

[E14] URL 编码与 Base64
来源：http://dxw.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dbi.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hei.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svl.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://npa.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jky.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xcj.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hiu.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rho.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://ubu.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://lks.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hmq.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nfu.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://big.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vyt.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://egd.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kpg.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhc.pycfn.com

[E16] 数字千分位
来源：http://gfw.uphjek.com

Py:   f"{1234567:,}"
来源：http://xbg.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://mae.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bsi.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ltp.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dje.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jal.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dwl.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://kea.ybcxt.top

[E17] 首字母大写
来源：http://cah.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ewy.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://spc.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nks.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uki.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://thu.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oic.ivvv.top

Ruby: s.capitalize
来源：http://yyj.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bhc.hnqzz.top

[E18] 模板占位符替换
来源：http://jra.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xnw.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wta.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rdu.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jtg.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://upa.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://quz.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ogj.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ugl.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://nte.shzxlz.cn

Py:   s.splitlines()
来源：http://bjd.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gmq.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://cvj.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://ccg.jianghu66.top

Java: s.lines().toList()
来源：http://tem.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://fzr.ctjpmb.com

Ruby: s.lines
来源：http://oii.daxiang520.top

C#:   s.Split('\n')
来源：http://oqx.zycfv.cn

[E20] 判断字符串是否为空
来源：http://jfs.yanxiufei.cn

Py:   if not s:
来源：http://zdb.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zpp.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cug.xuanzx.com

TS:   if (s === "") {}
来源：http://whv.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://ckj.ctjpmb.com

Go:   if s == "" {}
来源：http://xyh.fengsongda.top

Ruby: if s.empty?
来源：http://vps.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rel.dashuyun.cn

[E21] 超长截断加省略号
来源：http://sem.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rio.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pxf.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bps.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://whd.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ino.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://dpf.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vmo.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sgm.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://bmw.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://imf.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://irr.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ppz.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://svm.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://urn.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://khh.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://gai.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gjq.hywenlv.cn

================================================================================
来源：http://ovi.bbcook.cn

F. 文件与目录
来源：http://qnl.zhaomingkeji.xyz

================================================================================
来源：http://hkg.gaohongyu789.top

[F01] 读取整个文件
来源：http://ult.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ppt.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://pdw.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egs.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wxi.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ngi.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yco.iojbl.cn

Ruby: File.read("a.txt")
来源：http://sff.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://qtn.dianchejie.cn

[F02] 逐行读取文件
来源：http://wqa.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://flr.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://awc.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwb.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lwf.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gca.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lmm.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lum.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eeh.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://faq.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ava.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yjb.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqy.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bgu.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mdn.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xdi.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://eqc.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lsf.ppjwa.cn

[F04] 追加写入文件
来源：http://trw.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fnk.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gav.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imn.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qmj.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ulu.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://euz.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xuz.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lfx.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://smq.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lso.ivvv.top

PHP:  file_exists("a.txt");
来源：http://gpp.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://tij.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://mde.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wof.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bzk.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://fuo.yj20258.top

C#:   File.Exists("a.txt")
来源：http://nrn.9152youxi.cn

[F06] 删除文件
来源：http://fqj.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://olg.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://zhk.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://yqz.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bll.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qbv.yj20258.top

Go:   os.Remove("a.txt")
来源：http://lkz.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://env.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://mky.cashguo.top

[F07] 创建目录（含多级）
来源：http://grl.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lgv.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rex.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkv.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qlr.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ydj.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mpi.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eeq.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tjl.ydzc1.top

[F08] 遍历目录
来源：http://xjv.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yuj.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zam.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://dke.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://xks.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mev.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kvb.yongpay.top

Ruby: Dir.children("dir")
来源：http://yeb.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://rza.havefunace.top

[F09] 获取文件大小
来源：http://trz.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://xau.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://wyx.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://prw.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://qox.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tgv.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ihw.tanke756.top

Ruby: File.size("a.txt")
来源：http://mtt.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://mjd.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://jhr.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qij.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pjm.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://npp.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://imj.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ius.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzb.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fdf.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ieb.uphjek.com

[F11] 复制与移动文件
来源：http://don.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oax.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zsj.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lzc.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xzb.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jlp.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://juy.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yeu.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hmf.cashguo.top

[F12] CSV 读写
来源：http://xfa.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bkb.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mxd.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://roa.316326.xyz

TS:   // 同上
来源：http://qqs.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jkk.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oao.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mlj.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mur.redwolf501.top

================================================================================
来源：http://ryp.shanyushiyangtech.top

G. 面向对象
来源：http://mza.316326.xyz

================================================================================
来源：http://cki.uphjek.com

[G01] 定义类
来源：http://gne.ybcxt.top

Py:   class User: pass
来源：http://sle.pycfn.com

PHP:  class User {}
来源：http://lha.hongshengwenyu.top

JS:   class User {}
来源：http://zww.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://yfx.bjfxy.top

Java: class User {}
来源：http://piq.bbcook.cn

Go:   type User struct { Name string }
来源：http://ryr.chenlongwang.top

Ruby: class User; end
来源：http://eii.zhongyouzk.top

C#:   class User {}
来源：http://eoe.andypj.xyz

[G02] 构造函数
来源：http://lat.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://zgj.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://hto.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://ktz.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://oep.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://imw.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iuv.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://dlu.zycfv.cn


<!-- 参考信息 -->