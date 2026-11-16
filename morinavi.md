代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ceq.daxiang520.top

TS:   s.slice(1, 4)
来源：http://fcu.hammf.cn

Java: s.substring(1, 4)
来源：http://psf.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://avf.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://tuc.meibo888.top

C#:   s.Substring(1, 3)
来源：http://kbp.tianlin.xyz

[E04] 查找子串位置
来源：http://gla.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://jfv.yuxming.cn

PHP:  strpos($s, "x");
来源：http://veu.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wet.dashuyun.cn

TS:   s.indexOf("x")
来源：http://odi.xinyue.icu

Java: s.indexOf("x")
来源：http://cbm.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://mbp.jyoumei.cn

Ruby: s.index("x")
来源：http://zsh.cashguo.top

C#:   s.IndexOf("x")
来源：http://uxr.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ztj.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ehi.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://apu.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xzu.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fim.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zeo.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sqv.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rar.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zbr.zhaomingkeji.xyz

[E06] 替换子串
来源：http://sin.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bec.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://ozd.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vpp.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://cut.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkm.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gtd.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://box.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://rbf.tianlin.xyz

[E07] 按分隔符拆分
来源：http://nxd.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://alu.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jzy.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vxy.ppjwa.cn

TS:   s.split(",")
来源：http://lpg.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://txf.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kkz.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://ksm.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pac.cheryme.top

[E08] 数组按分隔符合并
来源：http://tcj.ppjwa.cn

Py:   ",".join(items)
来源：http://aec.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://lhu.snrcjt.cn

JS:   items.join(",")
来源：http://qzn.xuetiantiany.cn

TS:   items.join(",")
来源：http://puh.bjfxy.top

Java: String.join(",", items)
来源：http://zvp.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://ckb.vehdjk.com

Ruby: items.join(",")
来源：http://fkv.aibaodan.cn

C#:   string.Join(",", items)
来源：http://mbx.guowangkeji.top

[E09] 去除所有空白字符
来源：http://jsk.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://odt.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tmj.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://tma.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://gvp.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://emt.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cna.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://fjo.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dkw.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://umd.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cnq.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ozf.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://ovd.sweek.top

TS:   "7".padStart(3, "0")
来源：http://zby.xziqi.cn

Java: String.format("%03d", 7)
来源：http://yww.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://dcs.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bmi.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kqd.ehwqpu.com

[E11] 反转字符串
来源：http://ppp.yangfankeji.com

Py:   s[::-1]
来源：http://jjo.hesvh.cn

PHP:  strrev($s);
来源：http://axv.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://qwj.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://bum.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uyh.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iim.yuxming.cn

Ruby: s.reverse
来源：http://jxz.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dll.sweek.top

[E12] 统计某字符出现次数
来源：http://qxl.xylfe.cn

Py:   s.count("a")
来源：http://qcv.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://seq.jianghu66.top

JS:   s.split("a").length - 1
来源：http://jjl.fehbvm.com

TS:   s.split("a").length - 1
来源：http://xvh.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://czt.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://zxa.c1oappe.top

Ruby: s.count("a")
来源：http://luk.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://lwf.snrcjt.cn

[E13] 逐字符遍历
来源：http://smm.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://sjl.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wcw.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://afs.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://frq.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jdw.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mmh.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lwv.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wqt.xziqi.cn

[E14] URL 编码与 Base64
来源：http://jro.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zyq.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cek.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oaa.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fud.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sjr.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qep.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oge.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nfj.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://hbk.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oba.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://utg.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fli.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vgg.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dtq.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zsr.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ngq.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ntn.svipenyu.cn

[E16] 数字千分位
来源：http://fnc.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://ggx.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://ywc.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://suu.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ozg.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hdb.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qcb.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fdk.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://ssp.bbcook.cn

[E17] 首字母大写
来源：http://yrg.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mhu.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ixr.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://npy.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vnb.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dgp.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eln.snrcjt.cn

Ruby: s.capitalize
来源：http://cmq.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://msw.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://cfm.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://loa.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ljm.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gcd.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dqg.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ncq.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://euv.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dch.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aft.havefunace.top

[E19] 多行文本按行拆分
来源：http://kmb.shanyushiyangtech.top

Py:   s.splitlines()
来源：http://ldq.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pvm.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://rgv.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://rta.yongpay.top

Java: s.lines().toList()
来源：http://fca.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://hjy.hywenlv.cn

Ruby: s.lines
来源：http://tco.jinqigufen.top

C#:   s.Split('\n')
来源：http://vno.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://myp.shanyushiyangtech.top

Py:   if not s:
来源：http://pfc.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oyn.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zjy.jqgufenzy.top

TS:   if (s === "") {}
来源：http://xaj.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://pnl.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://rcs.0kj1m.cn

Ruby: if s.empty?
来源：http://zlw.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iqe.yongpay.top

[E21] 超长截断加省略号
来源：http://lwk.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gbq.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwg.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bng.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sri.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lbo.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://akd.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gos.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rqv.yvedp.cn

[E22] 字节长度与字符长度
来源：http://guu.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pzg.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qds.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jbf.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pxl.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jtq.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ezr.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://nud.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wdl.jqgfzy.top

================================================================================
来源：http://fzw.jyoumei.cn

F. 文件与目录
来源：http://pqx.jlsjyb.cn

================================================================================
来源：http://joo.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://qys.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xfo.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://jnm.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tro.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kyu.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gqm.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zss.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://fqj.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://pve.smart0.xyz

[F02] 逐行读取文件
来源：http://cui.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csb.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ktl.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yfh.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cil.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gwb.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fxi.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://emx.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hfc.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://tfr.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ita.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rap.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kun.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://clw.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cnv.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cpc.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://sox.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vjo.shzxlz.cn

[F04] 追加写入文件
来源：http://wri.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iyl.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qqs.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcs.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rkm.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bpo.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://csc.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bbd.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eth.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://jcj.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zlf.cashguo.top

PHP:  file_exists("a.txt");
来源：http://rnb.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://abw.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://wha.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mas.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vvy.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://jqa.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://pai.ctjpmb.com

[F06] 删除文件
来源：http://guf.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://oql.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://puu.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ouv.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://sea.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sar.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://swp.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://uln.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://ddk.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://uik.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nuy.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xyq.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://esj.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eld.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gox.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://htu.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ffh.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zwh.xinyue.icu

[F08] 遍历目录
来源：http://kni.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xpu.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zam.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://bbs.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://iqt.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tra.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vle.yvedp.cn

Ruby: Dir.children("dir")
来源：http://tvc.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://qzq.zhengqikj.top

[F09] 获取文件大小
来源：http://otj.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://fcc.smart0.xyz

PHP:  filesize("a.txt");
来源：http://upv.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://owh.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://uzk.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://lxz.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kig.xziqi.cn

Ruby: File.size("a.txt")
来源：http://run.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://bxs.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://pro.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bvu.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nat.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uyt.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://jpk.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oze.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zma.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ufs.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hti.ybcxt.top

[F11] 复制与移动文件
来源：http://clg.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qtg.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://stz.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yuq.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eqo.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ift.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sse.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rui.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ekc.uphjek.com

[F12] CSV 读写
来源：http://vio.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tci.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sbp.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ojm.zycfv.cn

TS:   // 同上
来源：http://cbn.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mdq.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxn.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hmw.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oes.sweek.top

================================================================================
来源：http://gdw.shanyushiyangtech.top

G. 面向对象
来源：http://efc.bjfxy.top

================================================================================
来源：http://esk.iojbl.cn

[G01] 定义类
来源：http://ghn.cucudq.cn

Py:   class User: pass
来源：http://acv.xuanzx.com

PHP:  class User {}
来源：http://tmx.tarul.cn

JS:   class User {}
来源：http://jrl.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://ozi.wangshuangyany.cn

Java: class User {}
来源：http://ixn.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://avh.0kj1m.cn

Ruby: class User; end
来源：http://fvi.smart0.xyz

C#:   class User {}
来源：http://aal.uphjek.com


<!-- 参考信息 -->