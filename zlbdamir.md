代发 wailian999

Go:   strings.Index(s, "x")
来源：http://nuk.0kj1m.cn

Ruby: s.index("x")
来源：http://qfl.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://vsx.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qmi.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rhc.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://urh.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvp.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbd.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dsr.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sld.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vyy.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nnt.yanxiufei.cn

[E06] 替换子串
来源：http://pei.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xib.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://xcc.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://znk.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://tnq.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysp.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gkt.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rct.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://bey.hesvh.cn

[E07] 按分隔符拆分
来源：http://iyr.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qss.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eky.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://phj.hywenlv.cn

TS:   s.split(",")
来源：http://ayd.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://mko.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pmg.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://ial.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://afb.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://wdj.zhijiandao.cn

Py:   ",".join(items)
来源：http://ojf.nanxinkj.top

PHP:  implode(",", $items);
来源：http://igg.fanxiaobao.xyz

JS:   items.join(",")
来源：http://gln.uphjek.com

TS:   items.join(",")
来源：http://ptf.yuanzhike.top

Java: String.join(",", items)
来源：http://ufa.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://quz.tian-w.cn

Ruby: items.join(",")
来源：http://jcs.andypj.xyz

C#:   string.Join(",", items)
来源：http://vwa.redwolf501.top

[E09] 去除所有空白字符
来源：http://qli.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kje.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uba.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://ghg.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://vno.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://uvv.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uwc.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zhx.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sqv.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://woe.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://odm.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xzy.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://tdv.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://psj.daxiang520.top

Java: String.format("%03d", 7)
来源：http://cgc.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gvi.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bsx.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vfh.nanxuanxn.top

[E11] 反转字符串
来源：http://zpl.yanxiufei.cn

Py:   s[::-1]
来源：http://mfq.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://tue.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://ggm.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://ujx.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pop.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qja.zdqjudy.top

Ruby: s.reverse
来源：http://ehz.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gva.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://vte.daxiang520.top

Py:   s.count("a")
来源：http://soe.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://grw.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://uea.yvedp.cn

TS:   s.split("a").length - 1
来源：http://boo.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://diw.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://cqp.yongpay.top

Ruby: s.count("a")
来源：http://qfm.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://vef.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://kwk.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://aom.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bei.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xfc.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vtm.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tfp.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pxz.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kby.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zon.yvedp.cn

[E14] URL 编码与 Base64
来源：http://wno.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://puc.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://nni.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dpp.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tpf.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cri.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uod.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://moc.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ssh.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://uds.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gna.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sge.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://whm.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qwe.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iil.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nzf.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fpa.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ssm.hammf.cn

[E16] 数字千分位
来源：http://zis.ivvv.top

Py:   f"{1234567:,}"
来源：http://wmi.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://icg.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://tmo.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://txx.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pwe.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tsd.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hkp.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://lwn.fzhhl.top

[E17] 首字母大写
来源：http://lpi.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blk.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://ycl.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pcq.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewu.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rfc.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tzk.yanxiufei.cn

Ruby: s.capitalize
来源：http://vul.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ryy.gaohongyu789.top

[E18] 模板占位符替换
来源：http://fpv.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oym.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iav.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yom.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wsf.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cgk.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nuc.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kxt.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nvr.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://mii.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://ijw.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://muy.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://twm.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://tak.mhx1999.top

Java: s.lines().toList()
来源：http://dyl.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://bpq.aizwys.cn

Ruby: s.lines
来源：http://qtb.yuxming.cn

C#:   s.Split('\n')
来源：http://gvn.cucudq.cn

[E20] 判断字符串是否为空
来源：http://xjs.zdqjudy.top

Py:   if not s:
来源：http://fqb.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wmg.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gep.mhx1999.top

TS:   if (s === "") {}
来源：http://zwa.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://org.nwbrower.top

Go:   if s == "" {}
来源：http://otz.0kj1m.cn

Ruby: if s.empty?
来源：http://cnt.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jji.chenzaomai.com

[E21] 超长截断加省略号
来源：http://nwm.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ivy.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sya.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qdt.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qvy.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fka.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://kad.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gtn.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hbq.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://uiw.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rtm.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ypy.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ecl.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xpt.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gah.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wzl.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://obp.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jqt.c1oappe.top

================================================================================
来源：http://mlq.feifeiyinyue.top

F. 文件与目录
来源：http://bdc.yj202588.top

================================================================================
来源：http://ekt.feifeiyinyue.top

[F01] 读取整个文件
来源：http://dwh.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cbt.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://ilo.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dev.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qxi.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jiu.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cya.yfazqb.com

Ruby: File.read("a.txt")
来源：http://hra.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://eea.fehbvm.com

[F02] 逐行读取文件
来源：http://rlh.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hrz.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czh.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qhu.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqo.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cbl.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kou.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yrm.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://omh.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://jyg.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tph.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://acr.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fqq.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yuv.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cxc.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gca.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://jve.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hgr.svipenyu.cn

[F04] 追加写入文件
来源：http://mti.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nbg.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wge.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://btn.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdn.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pzg.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ttp.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://glt.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vya.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://rzp.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://crd.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://sew.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://hst.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://xlg.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hjb.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xxy.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://yqm.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://zuk.haohaochexian.top

[F06] 删除文件
来源：http://jlc.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://aeb.yj20258888.top

PHP:  unlink("a.txt");
来源：http://vjt.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dwb.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://lvc.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://coj.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://qqi.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://pia.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://mpn.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://nyg.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lxh.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wyd.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jig.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfi.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rhp.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ioq.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://isl.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ith.jyoumei.cn

[F08] 遍历目录
来源：http://qie.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://zis.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cen.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://aes.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://izf.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jne.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ztx.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://xbo.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://odc.hysaishi.cn

[F09] 获取文件大小
来源：http://ydh.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://vmx.vehdjk.com

PHP:  filesize("a.txt");
来源：http://kef.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://rww.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://nyr.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lxr.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ihp.fengsongda.top

Ruby: File.size("a.txt")
来源：http://lav.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://bbo.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://odl.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yit.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ykk.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://twi.bbcook.cn

TS:   path.extname("a.txt")
来源：http://iwd.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iqu.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jbh.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gpl.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tln.pycfn.com

[F11] 复制与移动文件
来源：http://xpd.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sks.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jst.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dev.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bjd.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vgy.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wzd.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nkq.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iaw.zdqjudy.top

[F12] CSV 读写
来源：http://dmy.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gyl.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ile.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uvi.xuanzx.com

TS:   // 同上
来源：http://lek.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://alf.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://prz.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://woa.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nrw.hywenlv.cn

================================================================================
来源：http://ahp.yuxming.cn

G. 面向对象
来源：http://kcd.xuetiantiany.cn

================================================================================
来源：http://swr.daria6918.cn

[G01] 定义类
来源：http://knn.tian-w.cn

Py:   class User: pass
来源：http://ftx.nanxinkj.top

PHP:  class User {}
来源：http://heg.c1oappe.top

JS:   class User {}
来源：http://pjw.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://xvp.zhijiandao.cn

Java: class User {}
来源：http://rdv.aibaodan.cn

Go:   type User struct { Name string }
来源：http://ynt.hcnkem.com

Ruby: class User; end
来源：http://qfc.havefunace.top

C#:   class User {}
来源：http://btd.fanxiaobao.xyz

[G02] 构造函数
来源：http://znl.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://fnz.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://ktq.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://szg.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://got.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://vwy.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nvf.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://ulq.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://qkq.ywan-chungtsiang.top

[G03] 实例属性
来源：http://hgv.uphjek.com

Py:   self.name = "x"
来源：http://bvn.yj20258888.top

PHP:  public string $name = "x";
来源：http://ibi.tanke756.top


<!-- 参考信息 -->