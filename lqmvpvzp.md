代发 wailian999

[E06] 替换子串
来源：http://gfp.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gpd.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://mef.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgi.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://euo.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqr.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://upu.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://akg.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://nyf.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://hsc.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://asj.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dwh.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://sas.zhiwuduotai.top

TS:   s.split(",")
来源：http://uza.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pzd.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cyu.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://mxl.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mna.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://icr.tianlin.xyz

Py:   ",".join(items)
来源：http://owb.aibaodan.cn

PHP:  implode(",", $items);
来源：http://lvd.zhengqikj.top

JS:   items.join(",")
来源：http://gbv.xziqi.cn

TS:   items.join(",")
来源：http://uob.hcnkem.com

Java: String.join(",", items)
来源：http://spt.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://fug.gzhubu.top

Ruby: items.join(",")
来源：http://gkz.epnwcf.com

C#:   string.Join(",", items)
来源：http://lly.svipenyu.cn

[E09] 去除所有空白字符
来源：http://wxe.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cdw.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zze.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://heo.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://fxq.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://ort.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://qhg.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jfy.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zxv.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://emd.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cvf.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qke.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://gwp.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://yxf.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://dvu.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lwr.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://unx.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ivs.shangyingyoupin.top

[E11] 反转字符串
来源：http://xxk.epnwcf.com

Py:   s[::-1]
来源：http://hjq.jlsjyb.cn

PHP:  strrev($s);
来源：http://iyl.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://itx.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://mez.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ahr.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rmp.sufxvd.cn

Ruby: s.reverse
来源：http://uws.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://rvk.xinyue.icu

[E12] 统计某字符出现次数
来源：http://par.hfpthk.cn

Py:   s.count("a")
来源：http://zbw.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://cfd.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://ljd.52xcode.cn

TS:   s.split("a").length - 1
来源：http://drs.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lhb.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://vkd.hnxiangtu.top

Ruby: s.count("a")
来源：http://lhu.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://naf.zhixingplan.top

[E13] 逐字符遍历
来源：http://ogq.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://uiy.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfl.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://awn.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://are.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lmd.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ifg.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uwx.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://elh.yvedp.cn

[E14] URL 编码与 Base64
来源：http://voa.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fud.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvu.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xng.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zam.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ooi.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wtn.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fkq.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aan.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://tck.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rmq.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qwx.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dxj.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wec.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vdl.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tak.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sof.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xyu.52xcode.cn

[E16] 数字千分位
来源：http://bzr.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://zio.cdnleiting.top

PHP:  number_format(1234567);
来源：http://xfc.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hzt.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hcu.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pqa.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdg.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fyz.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://zop.uphjek.com

[E17] 首字母大写
来源：http://tty.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jib.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kts.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ecu.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsg.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mpr.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fdi.fktsv.cn

Ruby: s.capitalize
来源：http://uhj.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jqm.hnqzz.top

[E18] 模板占位符替换
来源：http://uhb.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ymm.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eyl.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pbc.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rof.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mgc.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pyp.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yul.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nye.guannengcc.top

[E19] 多行文本按行拆分
来源：http://ojd.dianchejie.cn

Py:   s.splitlines()
来源：http://low.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qop.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://wtw.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://igh.redwolf501.top

Java: s.lines().toList()
来源：http://ekc.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://tgv.shzxlz.cn

Ruby: s.lines
来源：http://euv.dashuyun.cn

C#:   s.Split('\n')
来源：http://chd.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://wiz.yuxming.cn

Py:   if not s:
来源：http://tja.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ezt.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mhk.vqdsnc.cn

TS:   if (s === "") {}
来源：http://yjc.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://jkt.nwbrower.top

Go:   if s == "" {}
来源：http://zne.smart0.xyz

Ruby: if s.empty?
来源：http://khv.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qum.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://wvi.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xkz.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xgy.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zty.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsu.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ptt.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://som.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ojc.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mzf.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://omr.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fbb.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gek.yangfankeji.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gqz.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gln.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zhe.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lpe.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://rrw.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://thz.fengsongda.top

================================================================================
来源：http://rhw.316326.xyz

F. 文件与目录
来源：http://ayw.redwolf501.top

================================================================================
来源：http://ktn.gzhubu.top

[F01] 读取整个文件
来源：http://tky.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eoz.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://jlq.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dnq.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kod.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ohz.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cro.sxryk.cn

Ruby: File.read("a.txt")
来源：http://snw.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://pmo.ybcxt.top

[F02] 逐行读取文件
来源：http://sin.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lpu.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fgy.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cvb.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tlm.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zme.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eqb.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xex.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lxy.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://wzq.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnw.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://svs.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pfi.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pmu.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ifx.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qhf.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://fnl.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gqo.jqgufenzy.top

[F04] 追加写入文件
来源：http://jtr.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gmh.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iyb.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfr.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ber.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dgh.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfq.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rdl.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cbi.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://jic.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jtn.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://tfo.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://chg.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://fhg.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://hyp.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eoj.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://yqk.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://itc.yuanzhike.top

[F06] 删除文件
来源：http://oxf.cashguo.top

Py:   os.remove("a.txt")
来源：http://mur.pycfn.com

PHP:  unlink("a.txt");
来源：http://lbm.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yrd.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ejb.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujv.uphjek.com

Go:   os.Remove("a.txt")
来源：http://gqs.ivvv.top

Ruby: File.delete("a.txt")
来源：http://red.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://llb.yvedp.cn

[F07] 创建目录（含多级）
来源：http://rtd.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jty.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://crl.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fle.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oei.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wrq.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tgd.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jta.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wkv.hfpthk.cn

[F08] 遍历目录
来源：http://wmx.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kwx.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ujw.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://kur.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://kul.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zxb.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xux.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://jxb.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://ubu.gotoacloud.top

[F09] 获取文件大小
来源：http://mwt.daria6918.cn

Py:   os.path.getsize("a.txt")
来源：http://oxp.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://cer.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://rtz.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://cur.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://egr.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zjv.smart0.xyz

Ruby: File.size("a.txt")
来源：http://ybh.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://akg.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://gth.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ibq.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qgt.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dsp.cheryme.top

TS:   path.extname("a.txt")
来源：http://tgw.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kam.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lpd.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xvx.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rme.haohaochexian.top

[F11] 复制与移动文件
来源：http://des.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vvh.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xqr.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvj.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bpw.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sjo.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nvi.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pkc.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://deu.wangshuangyany.cn

[F12] CSV 读写
来源：http://qpo.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jal.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mow.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zou.sweek.top

TS:   // 同上
来源：http://lmg.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bhu.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://guh.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dhi.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://myp.nanxuanxn.top

================================================================================
来源：http://nfr.hywenlv.cn

G. 面向对象
来源：http://gaw.shangyingyoupin.top

================================================================================
来源：http://fxm.ywan-chungtsiang.top

[G01] 定义类
来源：http://vtc.havefunace.top

Py:   class User: pass
来源：http://qal.kuanghao11.cn

PHP:  class User {}
来源：http://pfo.cucudq.cn

JS:   class User {}
来源：http://odr.ivvv.top

TS:   class User { name: string = ""; }
来源：http://spw.c1oappe.top

Java: class User {}
来源：http://dgr.gotoacloud.top

Go:   type User struct { Name string }
来源：http://fxg.nanxinkj.top

Ruby: class User; end
来源：http://ecp.yuanzhike.top

C#:   class User {}
来源：http://jkr.wangdashe.top

[G02] 构造函数
来源：http://tdr.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://uuw.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://vmg.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://gfe.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://bdw.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://ypw.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cmm.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://olc.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://jqa.sxryk.cn

[G03] 实例属性
来源：http://wxz.zdqjudy.top

Py:   self.name = "x"
来源：http://jea.yuanzhike.top

PHP:  public string $name = "x";
来源：http://lqo.birdmap.top

JS:   this.name = "x";
来源：http://xqk.birdmap.top

TS:   name: string = "x";
来源：http://mgx.zdbjq.cn

Java: private String name;
来源：http://szh.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://evx.svipenyu.cn

Ruby: @name = "x"
来源：http://ryu.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://sqc.gotoacloud.top

[G04] 定义方法
来源：http://qvc.nwbrower.top

Py:   def greet(self): return self.name
来源：http://gts.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nyv.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://ows.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://dzy.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://jtp.sweek.top


<!-- 参考信息 -->