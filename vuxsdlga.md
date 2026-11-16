代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oiu.zhoulong.xyz

[E03] 截取子串
来源：http://jbp.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://usk.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jyo.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://atf.hammf.cn

TS:   s.slice(1, 4)
来源：http://oqg.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://skd.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://guj.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://csw.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://vch.zycfv.cn

[E04] 查找子串位置
来源：http://izz.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://noc.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://zvy.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xgb.xuanzx.com

TS:   s.indexOf("x")
来源：http://fdf.zdqjudy.top

Java: s.indexOf("x")
来源：http://kwm.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://xot.yanxiufei.cn

Ruby: s.index("x")
来源：http://wki.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://tdo.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://env.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hdz.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://idh.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rct.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://vkc.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ilx.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cib.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xsx.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rmv.haohaochexian.top

[E06] 替换子串
来源：http://wdt.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cfn.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://ssp.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lii.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://ics.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ddp.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://scx.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ecq.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://ksj.redwolf501.top

[E07] 按分隔符拆分
来源：http://aiq.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oxu.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ati.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pgq.fktsv.cn

TS:   s.split(",")
来源：http://oei.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://gtb.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jwx.meibo888.top

Ruby: s.split(",");  s.split
来源：http://hcg.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sul.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://kdk.zhiwuduotai.top

Py:   ",".join(items)
来源：http://siy.yfazqb.com

PHP:  implode(",", $items);
来源：http://xvt.yuxming.cn

JS:   items.join(",")
来源：http://mco.pycfn.com

TS:   items.join(",")
来源：http://puj.fktsv.cn

Java: String.join(",", items)
来源：http://tul.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://eik.shangyingyoupin.top

Ruby: items.join(",")
来源：http://lrj.zdqjudy.top

C#:   string.Join(",", items)
来源：http://hdo.aibaodan.cn

[E09] 去除所有空白字符
来源：http://uqm.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfs.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kqu.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://mfv.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://umo.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://drh.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jlc.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qly.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qja.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://jmf.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bsn.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ikt.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://xal.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://akm.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://njc.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wpu.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dug.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lzj.shangyingyoupin.top

[E11] 反转字符串
来源：http://wca.yangfankeji.com

Py:   s[::-1]
来源：http://vgp.zhijiandao.cn

PHP:  strrev($s);
来源：http://zdp.cashguo.top

JS:   [...s].reverse().join("")
来源：http://mkm.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://yku.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vvt.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zrg.aibaodan.cn

Ruby: s.reverse
来源：http://tns.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://upu.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://mkd.cashguo.top

Py:   s.count("a")
来源：http://kaw.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://isl.bjfxy.top

JS:   s.split("a").length - 1
来源：http://vex.guannengcc.top

TS:   s.split("a").length - 1
来源：http://pih.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://umg.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://svu.yuxming.cn

Ruby: s.count("a")
来源：http://mij.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://qed.zdbjq.cn

[E13] 逐字符遍历
来源：http://qex.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://pfp.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yoe.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vij.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gxb.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ohc.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://afc.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gcz.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nqf.xylfe.cn

[E14] URL 编码与 Base64
来源：http://kny.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pmg.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zkq.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ekb.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hga.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iku.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baf.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yfn.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gxw.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://yxc.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://fiq.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xae.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ksq.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xlc.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nme.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://luk.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bmf.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ifw.fengsongda.top

[E16] 数字千分位
来源：http://zxc.ivvv.top

Py:   f"{1234567:,}"
来源：http://fja.nanxinkj.top

PHP:  number_format(1234567);
来源：http://nlj.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hpx.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://quv.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xil.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wcu.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ghi.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://vlr.yuxming.cn

[E17] 首字母大写
来源：http://sbt.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vol.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bym.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://khk.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bmu.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ils.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nvk.birdmap.top

Ruby: s.capitalize
来源：http://bpy.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zzr.dashuyun.cn

[E18] 模板占位符替换
来源：http://gow.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ftt.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hse.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://akj.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jlc.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://agw.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ciz.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pfj.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wgn.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://qcs.hammf.cn

Py:   s.splitlines()
来源：http://fco.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qia.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://mly.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://tar.bbcook.cn

Java: s.lines().toList()
来源：http://zsj.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://bca.daxiang520.top

Ruby: s.lines
来源：http://rnk.ydjk.org.cn

C#:   s.Split('\n')
来源：http://nhr.iojbl.cn

[E20] 判断字符串是否为空
来源：http://fpd.zhixingplan.top

Py:   if not s:
来源：http://myz.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://flu.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zzr.hnqzz.top

TS:   if (s === "") {}
来源：http://vwj.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://onr.mhx1999.top

Go:   if s == "" {}
来源：http://cdh.redwolf501.top

Ruby: if s.empty?
来源：http://fxc.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://exf.sysykeji.top

[E21] 超长截断加省略号
来源：http://tbm.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zyr.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pxr.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkz.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dva.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yjy.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://dua.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fqi.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ntr.fehbvm.com

[E22] 字节长度与字符长度
来源：http://atx.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://utl.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://coy.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://upo.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ppn.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://heh.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vug.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://ijz.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zlk.xylfe.cn

================================================================================
来源：http://wbp.ydjk.org.cn

F. 文件与目录
来源：http://etl.yongpay.top

================================================================================
来源：http://mvj.mhx1999.top

[F01] 读取整个文件
来源：http://qqm.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vpc.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://yml.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://one.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tzl.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wuw.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pea.epnwcf.com

Ruby: File.read("a.txt")
来源：http://fax.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://zxl.hesvh.cn

[F02] 逐行读取文件
来源：http://tqt.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pmz.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wbz.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ycx.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iuu.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hmm.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ggk.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cek.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xck.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://nxy.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kgu.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qiq.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sow.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bnh.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lfe.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://owf.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://yar.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://trt.gaohongyu789.top

[F04] 追加写入文件
来源：http://isu.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gcy.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yaq.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hwg.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fns.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sai.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ayd.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://haq.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ssr.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://jqn.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kml.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://edk.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://qpj.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://zkf.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kpo.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nia.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://dcx.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://tgl.vqdsnc.cn

[F06] 删除文件
来源：http://rvw.yj20258888.top

Py:   os.remove("a.txt")
来源：http://gzf.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://mhq.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rtt.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://dwv.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nsc.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://iay.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://njc.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://sjb.andypj.xyz

[F07] 创建目录（含多级）
来源：http://liy.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lqj.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bgf.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhn.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xpq.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rwb.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bgu.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jhh.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gjk.guannengcc.top

[F08] 遍历目录
来源：http://atx.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://hvc.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lze.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://dck.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://cez.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bgf.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kyl.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://fab.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://wql.yuanzhike.top

[F09] 获取文件大小
来源：http://qiq.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://xsq.c1oappe.top

PHP:  filesize("a.txt");
来源：http://eio.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://cia.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://mxf.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zwd.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hdl.yvedp.cn

Ruby: File.size("a.txt")
来源：http://xdz.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://udc.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://wmh.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vfc.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qdb.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wmk.havefunace.top

TS:   path.extname("a.txt")
来源：http://eiu.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jaf.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mek.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ers.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kgx.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://xsg.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xtf.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eno.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fwp.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qei.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xpx.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mff.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://thv.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cgc.jqgufenzy.top

[F12] CSV 读写
来源：http://ocb.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yhn.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gbs.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eib.yangfankeji.com

TS:   // 同上
来源：http://atv.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hqj.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cpj.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zro.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://dpt.shuidangran.top

================================================================================
来源：http://hhl.zhoulong.xyz

G. 面向对象
来源：http://lih.hesvh.cn

================================================================================
来源：http://yaq.redwolf501.top

[G01] 定义类
来源：http://bva.daxiang520.top

Py:   class User: pass
来源：http://lde.meibo888.top

PHP:  class User {}
来源：http://yam.yonumen.top

JS:   class User {}
来源：http://wgj.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://gjb.ydzc1.top


<!-- 参考信息 -->