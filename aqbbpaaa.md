代发 wailian999

Go:   strings.Index(s, "x")
来源：http://bnr.fengsongda.top

Ruby: s.index("x")
来源：http://ede.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://exj.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uje.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eti.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jtv.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmu.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://mzp.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ngf.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qqa.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://afo.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vky.jinyuanbaomall.cn

[E06] 替换子串
来源：http://ops.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://maa.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://upc.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://msc.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://snd.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oos.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dlo.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rue.hammf.cn

C#:   s.Replace("a", "b")
来源：http://wgd.fzhhl.top

[E07] 按分隔符拆分
来源：http://kir.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aef.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://deq.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rcm.snrcjt.cn

TS:   s.split(",")
来源：http://ifm.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://rmf.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jow.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://ggd.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yjy.ybcxt.top

[E08] 数组按分隔符合并
来源：http://kwv.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://hko.ivvv.top

PHP:  implode(",", $items);
来源：http://vdp.jlsjyb.cn

JS:   items.join(",")
来源：http://hdy.yj20258888.top

TS:   items.join(",")
来源：http://cro.9152youxi.cn

Java: String.join(",", items)
来源：http://lgq.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://dup.jinqigfzy.top

Ruby: items.join(",")
来源：http://bnj.cdnleiting.top

C#:   string.Join(",", items)
来源：http://giq.tarul.cn

[E09] 去除所有空白字符
来源：http://fzw.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zdi.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://taq.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://dch.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://sol.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://rvr.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wxp.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://bxg.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ubz.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://wew.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qcl.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ioq.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://enc.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://ias.yfazqb.com

Java: String.format("%03d", 7)
来源：http://qnq.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vxq.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kie.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xsn.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://jsh.haohaochexian.top

Py:   s[::-1]
来源：http://oet.tarul.cn

PHP:  strrev($s);
来源：http://vey.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://cmq.pycfn.com

TS:   [...s].reverse().join("")
来源：http://rgt.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xax.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://uwf.hammf.cn

Ruby: s.reverse
来源：http://vel.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nem.yongpay.top

[E12] 统计某字符出现次数
来源：http://bab.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://cvm.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://cya.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://upt.yj20258888.top

TS:   s.split("a").length - 1
来源：http://zfi.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rev.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://xtd.cdnleiting.top

Ruby: s.count("a")
来源：http://rxh.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://ies.ehwqpu.com

[E13] 逐字符遍历
来源：http://nac.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://wgq.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pza.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jci.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fzy.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gqr.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mum.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rcd.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wsv.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://uzh.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bqs.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://vyq.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nbw.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yel.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rri.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cjl.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qwm.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ovz.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://tme.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vkk.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gid.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kbr.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://grr.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xug.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hyl.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fcj.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://drz.xinyue.icu

[E16] 数字千分位
来源：http://iwa.xylfe.cn

Py:   f"{1234567:,}"
来源：http://okw.yangfankeji.com

PHP:  number_format(1234567);
来源：http://yph.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://esl.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://osk.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yus.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vro.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rjf.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://gty.zdqjudy.top

[E17] 首字母大写
来源：http://bdl.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zle.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vkh.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://suq.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jks.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wml.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://efh.zhiwuduotai.top

Ruby: s.capitalize
来源：http://ovl.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qxs.zhongyouzk.top

[E18] 模板占位符替换
来源：http://umb.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zoo.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://twp.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://blh.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hnn.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jel.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iwg.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rhx.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://akh.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://asu.mhx1999.top

Py:   s.splitlines()
来源：http://vfy.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uku.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://aeh.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://oco.ydzc1.top

Java: s.lines().toList()
来源：http://xha.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://ynh.fzhhl.top

Ruby: s.lines
来源：http://qvw.tianlin.xyz

C#:   s.Split('\n')
来源：http://wnc.xuanzx.com

[E20] 判断字符串是否为空
来源：http://btz.jqgufenzy.top

Py:   if not s:
来源：http://hxx.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://caw.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lrc.ivvv.top

TS:   if (s === "") {}
来源：http://xxe.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://zki.daria6918.cn

Go:   if s == "" {}
来源：http://avo.shzxlz.cn

Ruby: if s.empty?
来源：http://mwy.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aei.gogol.net.cn

[E21] 超长截断加省略号
来源：http://zds.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ymp.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tky.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfr.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ewr.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hzx.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://hyy.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oqh.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://isz.c1oappe.top

[E22] 字节长度与字符长度
来源：http://xqp.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://exj.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tah.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nay.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jxl.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kip.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xje.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://vzp.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mqr.bjfxy.top

================================================================================
来源：http://hoa.hcnkem.com

F. 文件与目录
来源：http://vvb.epnwcf.com

================================================================================
来源：http://mhe.yanxiufei.cn

[F01] 读取整个文件
来源：http://uzq.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ebe.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://vhm.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ssr.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fto.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pll.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yyh.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://kcp.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://fvl.chenzaomai.com

[F02] 逐行读取文件
来源：http://pso.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vyc.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rvi.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qks.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://djc.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nxv.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xue.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ahl.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bqt.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://vuu.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ijj.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbk.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qmq.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akw.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pdp.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rpc.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://yuh.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cpz.epnwcf.com

[F04] 追加写入文件
来源：http://uwm.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jsa.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://osy.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfl.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afb.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zgz.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vjp.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aan.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hyo.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://rsh.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mej.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://wzm.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://pch.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://ufl.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zed.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zge.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://oay.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://ixy.bjfxy.top

[F06] 删除文件
来源：http://aqx.iojbl.cn

Py:   os.remove("a.txt")
来源：http://ztb.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://cab.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://epg.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rph.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://udd.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://hto.birdmap.top

Ruby: File.delete("a.txt")
来源：http://wmb.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://bfh.smart0.xyz

[F07] 创建目录（含多级）
来源：http://bdg.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xhy.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gzh.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jtw.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gnj.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qoo.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ijn.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://scq.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qnv.zdqjudy.top

[F08] 遍历目录
来源：http://jjw.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zlb.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hzz.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://qre.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://rnr.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cga.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qgy.redwolf501.top

Ruby: Dir.children("dir")
来源：http://vxh.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://ocv.mhx1999.top

[F09] 获取文件大小
来源：http://hys.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://iom.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://ads.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://drr.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://yii.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://fkn.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ijf.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://pbl.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://wmn.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://vce.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cua.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://con.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dsi.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://ffp.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hyd.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aec.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dxq.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xzr.jyoumei.cn

[F11] 复制与移动文件
来源：http://ffn.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fnn.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dhk.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://deb.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xtm.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ybq.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bbp.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vob.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wil.kuanghao11.cn

[F12] CSV 读写
来源：http://tkn.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xxh.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cuc.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cka.sysykeji.top

TS:   // 同上
来源：http://zhg.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ahb.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ohk.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hsl.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ngf.sxryk.cn

================================================================================
来源：http://ymk.fanxiaobao.xyz

G. 面向对象
来源：http://clf.yuxming.cn

================================================================================
来源：http://dqh.pycfn.com

[G01] 定义类
来源：http://nga.jinqigfzy.top

Py:   class User: pass
来源：http://dmn.mhx1999.top

PHP:  class User {}
来源：http://bgn.bjfxy.top

JS:   class User {}
来源：http://utn.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://mzu.aibaodan.cn

Java: class User {}
来源：http://qqp.birdmap.top

Go:   type User struct { Name string }
来源：http://hdt.sufxvd.cn

Ruby: class User; end
来源：http://ita.ehwqpu.com

C#:   class User {}
来源：http://mpc.guannengcc.top

[G02] 构造函数
来源：http://tpy.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://wfv.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://rpi.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://nct.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://gxe.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://agg.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nln.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://jje.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://ufj.pengpengdd.cyou

[G03] 实例属性
来源：http://jnu.xylfe.cn

Py:   self.name = "x"
来源：http://xtb.yvedp.cn

PHP:  public string $name = "x";
来源：http://jmk.tanke756.top


<!-- 参考信息 -->