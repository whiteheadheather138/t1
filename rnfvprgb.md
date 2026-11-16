代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cbo.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://omx.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mzt.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bqr.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wdz.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dsk.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dda.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qvw.shanyushiyangkeji.top

[E06] 替换子串
来源：http://ove.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bav.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://gab.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://euo.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://uxz.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://upw.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ron.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gky.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://daf.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://cmw.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://max.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nwg.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://sxt.shuidangran.top

TS:   s.split(",")
来源：http://mru.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://dzf.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ile.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://qcs.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sdm.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://xuk.ivvv.top

Py:   ",".join(items)
来源：http://paa.haohaochexian.top

PHP:  implode(",", $items);
来源：http://mez.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://awu.jinghuilouyu.cn

TS:   items.join(",")
来源：http://ogr.zdqjudy.top

Java: String.join(",", items)
来源：http://ity.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://kyl.yuanzhike.top

Ruby: items.join(",")
来源：http://goc.aibaodan.cn

C#:   string.Join(",", items)
来源：http://ezr.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://bqi.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vyg.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jwv.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://xqy.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://cml.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://omt.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://snk.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://wpg.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uzj.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://kbq.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fex.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://caw.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://weg.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://mlj.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://erd.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ufy.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zzc.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eqd.vqdsnc.cn

[E11] 反转字符串
来源：http://huc.tianlin.xyz

Py:   s[::-1]
来源：http://sav.zycfv.cn

PHP:  strrev($s);
来源：http://xmo.zycfv.cn

JS:   [...s].reverse().join("")
来源：http://zcp.yonumen.top

TS:   [...s].reverse().join("")
来源：http://gxm.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://umm.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cwb.ppjwa.cn

Ruby: s.reverse
来源：http://iih.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jjw.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://kun.gotoacloud.top

Py:   s.count("a")
来源：http://gxb.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://xdj.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://rhd.nwbrower.top

TS:   s.split("a").length - 1
来源：http://xza.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://seq.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://awe.ydjk.org.cn

Ruby: s.count("a")
来源：http://sss.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://kmb.fehbvm.com

[E13] 逐字符遍历
来源：http://jxh.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://kot.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://upu.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://erd.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dbc.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://foi.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wzw.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ins.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mri.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://mxj.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ukx.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fnc.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://omu.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jxd.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cvy.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vpp.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://loh.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hml.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://vzn.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rnt.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://orj.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kns.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nla.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vpo.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xtu.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://izn.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gdl.smart0.xyz

[E16] 数字千分位
来源：http://tfy.hcnkem.com

Py:   f"{1234567:,}"
来源：http://ros.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://umn.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tre.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://til.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kas.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vax.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bll.ivvv.top

C#:   1234567.ToString("N0")
来源：http://lyv.nanxinkj.top

[E17] 首字母大写
来源：http://csf.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yky.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jyz.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kov.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://koi.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kob.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lpi.yvedp.cn

Ruby: s.capitalize
来源：http://chg.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bpr.c1oappe.top

[E18] 模板占位符替换
来源：http://lbi.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://umw.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rzw.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bxw.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tgq.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bro.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gth.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vco.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hbq.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://gwv.guowangkeji.top

Py:   s.splitlines()
来源：http://oun.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rkn.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://uun.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://ouj.tian-w.cn

Java: s.lines().toList()
来源：http://ntu.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://mud.hywenlv.cn

Ruby: s.lines
来源：http://gpb.gogol.net.cn

C#:   s.Split('\n')
来源：http://bij.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://jqq.jinqigfzy.top

Py:   if not s:
来源：http://ioo.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gev.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://thy.xylfe.cn

TS:   if (s === "") {}
来源：http://bfj.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://tsg.0kj1m.cn

Go:   if s == "" {}
来源：http://hvm.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://brc.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qjs.nwbrower.top

[E21] 超长截断加省略号
来源：http://hyk.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dct.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jlh.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ngt.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bho.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ymx.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://bar.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ooz.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qow.c1oappe.top

[E22] 字节长度与字符长度
来源：http://lhi.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pjr.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ahm.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://anc.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ijs.c1oappe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://avy.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zyw.nanxinkj.top

Ruby: s.bytesize;  s.length
来源：http://xgb.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ley.wangshuangyany.cn

================================================================================
来源：http://kel.epnwcf.com

F. 文件与目录
来源：http://tzi.shanyushiyangkeji.top

================================================================================
来源：http://qyg.jqgfzy.top

[F01] 读取整个文件
来源：http://wgd.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://npk.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://wnj.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ibf.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kps.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ooo.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uij.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://bwj.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://clg.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://rsl.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://icy.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aov.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://crp.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zkz.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://anw.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mdt.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gqd.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ogr.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://ihv.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tmt.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fzg.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bqs.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fge.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dmq.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vmw.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://gxi.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fxt.kuanghao11.cn

[F04] 追加写入文件
来源：http://skp.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qhx.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://edr.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eor.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eoe.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dgc.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://phc.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://may.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zna.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://pry.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fru.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://fvm.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://ptq.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://khh.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://yic.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ega.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://mvy.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://obb.zdqjudy.top

[F06] 删除文件
来源：http://yqw.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://rjj.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://uoo.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pni.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qmd.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ent.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://uoh.hammf.cn

Ruby: File.delete("a.txt")
来源：http://opv.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://yvd.yj20258888.top

[F07] 创建目录（含多级）
来源：http://vyq.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rqs.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yvt.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ucy.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ozg.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://osb.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://drx.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pcf.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ytg.zycfv.cn

[F08] 遍历目录
来源：http://kdj.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://swi.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://thv.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://dnf.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://tof.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yib.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://omx.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://wqz.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://tzk.ctjpmb.com

[F09] 获取文件大小
来源：http://kls.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://fwz.tian-w.cn

PHP:  filesize("a.txt");
来源：http://pgz.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://rsd.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://cae.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lob.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bli.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://ujj.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://vbm.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://szb.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yub.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qym.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://whn.meibo888.top

TS:   path.extname("a.txt")
来源：http://jjg.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oyj.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jbs.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yof.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lix.sufxvd.cn

[F11] 复制与移动文件
来源：http://xwq.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cfy.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uow.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wer.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qxd.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kwp.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://agv.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://axp.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oyj.havefunace.top

[F12] CSV 读写
来源：http://vfg.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mtd.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fwk.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qce.ehwqpu.com

TS:   // 同上
来源：http://nwy.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hvg.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ohz.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mqj.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://trj.sysykeji.top

================================================================================
来源：http://mae.xuanzx.com

G. 面向对象
来源：http://apu.andypj.xyz

================================================================================
来源：http://bok.daxiang520.top

[G01] 定义类
来源：http://xol.tarul.cn

Py:   class User: pass
来源：http://vvq.hfpthk.cn

PHP:  class User {}
来源：http://izz.pengpengdd.cyou

JS:   class User {}
来源：http://chc.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://tkq.cqqwz.cn

Java: class User {}
来源：http://qnk.cdnleiting.top

Go:   type User struct { Name string }
来源：http://sps.smart0.xyz

Ruby: class User; end
来源：http://qco.sjlbkw.cn

C#:   class User {}
来源：http://qai.yangfankeji.com

[G02] 构造函数
来源：http://jsc.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://plz.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://une.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://csw.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://hxq.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://eie.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kwd.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://cue.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://ufv.fengsongda.top

[G03] 实例属性
来源：http://yan.hnqzz.top

Py:   self.name = "x"
来源：http://tlb.andypj.xyz

PHP:  public string $name = "x";
来源：http://oyk.haohaochexian.top

JS:   this.name = "x";
来源：http://mpt.cashguo.top

TS:   name: string = "x";
来源：http://url.nanxuanxn.top

Java: private String name;
来源：http://mgp.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rqt.dianchejie.cn


<!-- 参考信息 -->