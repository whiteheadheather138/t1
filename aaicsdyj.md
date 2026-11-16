代发 wailian999

Go:   strings.Index(s, "x")
来源：http://zov.hnqzz.top

Ruby: s.index("x")
来源：http://peu.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://vtz.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://czf.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xxi.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://grm.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://caw.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gvo.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kmv.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sak.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hxn.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yjg.316326.xyz

[E06] 替换子串
来源：http://oab.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iep.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://kzz.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://svv.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://ews.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mfi.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kxu.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://afp.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://zzi.ppjwa.cn

[E07] 按分隔符拆分
来源：http://aox.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wov.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://woi.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dlv.yfazqb.com

TS:   s.split(",")
来源：http://mwa.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ahg.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://feg.hammf.cn

Ruby: s.split(",");  s.split
来源：http://mwa.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zeh.iojbl.cn

[E08] 数组按分隔符合并
来源：http://zpz.hnqzz.top

Py:   ",".join(items)
来源：http://uzb.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://upi.gotoacloud.top

JS:   items.join(",")
来源：http://xgn.mhx1999.top

TS:   items.join(",")
来源：http://pgs.shuidangran.top

Java: String.join(",", items)
来源：http://tbm.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://fwi.zhijiandao.cn

Ruby: items.join(",")
来源：http://hvp.316326.xyz

C#:   string.Join(",", items)
来源：http://tbb.ydzc1.top

[E09] 去除所有空白字符
来源：http://nhp.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yrq.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://efh.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://ieg.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://wiq.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://pfp.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lep.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://asj.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yoo.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://cxn.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uns.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jpi.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://skg.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://aig.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://ane.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ntm.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hkw.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://puj.birdmap.top

[E11] 反转字符串
来源：http://fnl.guannengcc.top

Py:   s[::-1]
来源：http://hzk.uphjek.com

PHP:  strrev($s);
来源：http://hkw.havefunace.top

JS:   [...s].reverse().join("")
来源：http://nso.hammf.cn

TS:   [...s].reverse().join("")
来源：http://fbt.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ifm.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tdg.jinqigfzy.top

Ruby: s.reverse
来源：http://zyt.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://nxw.gzhubu.top

[E12] 统计某字符出现次数
来源：http://pwk.gogol.net.cn

Py:   s.count("a")
来源：http://myj.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://aoc.gzhubu.top

JS:   s.split("a").length - 1
来源：http://bmu.fzhhl.top

TS:   s.split("a").length - 1
来源：http://jnh.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dmx.pycfn.com

Go:   strings.Count(s, "a")
来源：http://blh.bjfxy.top

Ruby: s.count("a")
来源：http://nin.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://rzx.0kj1m.cn

[E13] 逐字符遍历
来源：http://bab.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://zky.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhn.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qhb.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qoi.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fgh.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pbm.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://blq.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xmg.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://fpg.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zbh.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qad.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wrw.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tkn.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jkp.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qzh.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://azs.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wrp.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://zqq.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jzv.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://emx.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kfu.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yap.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yzx.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mla.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lcx.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ghd.zdbjq.cn

[E16] 数字千分位
来源：http://pmn.xziqi.cn

Py:   f"{1234567:,}"
来源：http://haj.redwolf501.top

PHP:  number_format(1234567);
来源：http://age.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dwh.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oac.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://elo.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fal.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qix.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://rhn.daria6918.cn

[E17] 首字母大写
来源：http://evf.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tgj.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dxa.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xgn.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfp.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yvf.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mwb.cdnleiting.top

Ruby: s.capitalize
来源：http://xlb.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://whl.c1oappe.top

[E18] 模板占位符替换
来源：http://vzq.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fah.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsc.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jck.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://tlj.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wvl.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://glr.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://edv.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zbl.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://skb.bbcook.cn

Py:   s.splitlines()
来源：http://teh.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mgy.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://lpw.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://dnc.ppjwa.cn

Java: s.lines().toList()
来源：http://wyf.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://uxo.jiagoushi.top

Ruby: s.lines
来源：http://vub.sxryk.cn

C#:   s.Split('\n')
来源：http://izq.sxryk.cn

[E20] 判断字符串是否为空
来源：http://ltn.ydjk.org.cn

Py:   if not s:
来源：http://pks.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dwz.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rdk.gaohongyu789.top

TS:   if (s === "") {}
来源：http://eaq.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://fsm.bjfxy.top

Go:   if s == "" {}
来源：http://paa.pengpengdd.cyou

Ruby: if s.empty?
来源：http://lkj.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jvd.daxiang520.top

[E21] 超长截断加省略号
来源：http://ygr.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gxj.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcb.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nfy.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bdm.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bpp.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://nov.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kcm.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cws.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://unx.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jrs.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uda.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sxq.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tuy.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ivl.ydjk.org.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xly.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://xgs.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://glw.aizwys.cn

================================================================================
来源：http://auh.feifeiyinyue.top

F. 文件与目录
来源：http://xys.yvedp.cn

================================================================================
来源：http://dnc.hammf.cn

[F01] 读取整个文件
来源：http://uty.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nxm.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://dzm.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lfp.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gsx.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kbl.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vdq.uphjek.com

Ruby: File.read("a.txt")
来源：http://oiv.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://iwy.andypj.xyz

[F02] 逐行读取文件
来源：http://het.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://izq.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uwm.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oac.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://anf.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qbn.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hpg.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://psf.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xcc.cheryme.top

[F03] 写入文件（覆盖）
来源：http://ben.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rne.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ldf.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://znw.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qja.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tvk.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pba.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://uya.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ayz.gzhubu.top

[F04] 追加写入文件
来源：http://mwc.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zlr.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sbn.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfv.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jzr.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xtt.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lyd.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lbj.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jyb.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://iph.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xzd.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://ifn.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://bwr.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://vzu.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://foi.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vyo.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://huz.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://qgj.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://uhb.gzhubu.top

Py:   os.remove("a.txt")
来源：http://xcn.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://oot.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://ibb.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://msk.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fqg.pycfn.com

Go:   os.Remove("a.txt")
来源：http://dux.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://hji.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://gox.tanke756.top

[F07] 创建目录（含多级）
来源：http://tfo.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://did.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ufh.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvp.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ccb.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ksw.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ovd.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fvj.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://okv.epnwcf.com

[F08] 遍历目录
来源：http://hmd.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wvi.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://saj.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://pgn.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://ltd.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ikv.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qji.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://zzz.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://zet.shuidangran.top

[F09] 获取文件大小
来源：http://azl.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://qql.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://zvf.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://rbs.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://pmk.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://ian.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://axn.xinyue.icu

Ruby: File.size("a.txt")
来源：http://zra.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://yse.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://ijt.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xsq.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uip.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fjy.yongpay.top

TS:   path.extname("a.txt")
来源：http://cbr.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oqt.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kpc.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sdl.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uyi.ydjk.org.cn

[F11] 复制与移动文件
来源：http://bed.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jbg.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xhs.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://avz.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdo.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nlx.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lcw.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://slx.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yvh.hfpthk.cn

[F12] CSV 读写
来源：http://rfz.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://opc.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gvq.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jqy.yueranfly.top

TS:   // 同上
来源：http://rdy.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kes.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qoz.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bfa.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hjd.tarul.cn

================================================================================
来源：http://ssf.aibaodan.cn

G. 面向对象
来源：http://emc.snrcjt.cn

================================================================================
来源：http://erw.sysykeji.top

[G01] 定义类
来源：http://vqq.ehwqpu.com

Py:   class User: pass
来源：http://ztg.wangshuangyany.cn

PHP:  class User {}
来源：http://ozb.ydjk.org.cn

JS:   class User {}
来源：http://iih.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://lul.xinyue.icu

Java: class User {}
来源：http://hac.svipenyu.cn

Go:   type User struct { Name string }
来源：http://bmb.zhengqikj.top

Ruby: class User; end
来源：http://exu.ywan-chungtsiang.top

C#:   class User {}
来源：http://ddm.hfpthk.cn

[G02] 构造函数
来源：http://owq.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://oyl.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://oae.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://mwx.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://ahd.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://wcv.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://unq.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://jlp.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://vdj.gzhubu.top

[G03] 实例属性
来源：http://lyz.fehbvm.com

Py:   self.name = "x"
来源：http://siq.cqqwz.cn

PHP:  public string $name = "x";
来源：http://kix.svipenyu.cn


<!-- 参考信息 -->