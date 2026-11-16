代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rdf.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tab.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kyx.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://apl.jinghuilouyu.cn

[E06] 替换子串
来源：http://ccg.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ihq.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://ptz.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iws.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://lgb.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uzk.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://apu.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aix.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://iru.hcnkem.com

[E07] 按分隔符拆分
来源：http://hor.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rzn.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wae.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://epy.snrcjt.cn

TS:   s.split(",")
来源：http://cla.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://was.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fwm.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://bpy.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://giz.yongpay.top

[E08] 数组按分隔符合并
来源：http://mos.c1oappe.top

Py:   ",".join(items)
来源：http://hrf.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://sxe.nanxinkj.top

JS:   items.join(",")
来源：http://spf.cqqwz.cn

TS:   items.join(",")
来源：http://lds.hysaishi.cn

Java: String.join(",", items)
来源：http://ble.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://rit.cdnleiting.top

Ruby: items.join(",")
来源：http://pxz.sufxvd.cn

C#:   string.Join(",", items)
来源：http://rev.hesvh.cn

[E09] 去除所有空白字符
来源：http://mqb.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dvl.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zfh.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://hkv.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://bob.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://hvp.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://knv.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tst.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jly.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://pzt.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qxw.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mch.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://trl.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://hve.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://ejd.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ifc.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xjq.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fkb.hfpthk.cn

[E11] 反转字符串
来源：http://dnb.sysykeji.top

Py:   s[::-1]
来源：http://hdj.jianghu66.top

PHP:  strrev($s);
来源：http://ngs.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://rvx.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://bjb.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qfl.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://vke.yangfankeji.com

Ruby: s.reverse
来源：http://xwq.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://tzf.0kj1m.cn

[E12] 统计某字符出现次数
来源：http://rkw.jyoumei.cn

Py:   s.count("a")
来源：http://rfl.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://ems.yongpay.top

JS:   s.split("a").length - 1
来源：http://ycf.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://bsh.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tct.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://llb.tianlin.xyz

Ruby: s.count("a")
来源：http://ntc.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://vtn.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://aok.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://oij.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvn.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://frh.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ogy.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gel.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sgc.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wsh.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ipd.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://kin.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hcr.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ksk.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ucb.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oiv.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yrv.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yij.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blr.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nal.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://jge.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dii.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ffl.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vev.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://xic.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcm.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qpl.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ayf.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qro.jyoumei.cn

[E16] 数字千分位
来源：http://tcg.yfazqb.com

Py:   f"{1234567:,}"
来源：http://dlz.haohaochexian.top

PHP:  number_format(1234567);
来源：http://aeu.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ktm.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xsb.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ron.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://arv.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://doz.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://mvi.ivvv.top

[E17] 首字母大写
来源：http://qjh.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jcb.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://brx.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://urx.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qka.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aie.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://viy.andypj.xyz

Ruby: s.capitalize
来源：http://cxi.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lwq.birdmap.top

[E18] 模板占位符替换
来源：http://afq.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ujt.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zom.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kno.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://trf.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfn.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://per.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nzt.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jiy.cucudq.cn

[E19] 多行文本按行拆分
来源：http://dfw.nanxinkj.top

Py:   s.splitlines()
来源：http://qbi.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tqm.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://svk.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://occ.nanxinkj.top

Java: s.lines().toList()
来源：http://doi.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://nxm.vehdjk.com

Ruby: s.lines
来源：http://ccv.0kj1m.cn

C#:   s.Split('\n')
来源：http://ggc.yongpay.top

[E20] 判断字符串是否为空
来源：http://wwd.0kj1m.cn

Py:   if not s:
来源：http://pto.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pgl.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cwk.sjlbkw.cn

TS:   if (s === "") {}
来源：http://xno.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://kri.tian-w.cn

Go:   if s == "" {}
来源：http://ifi.ctjpmb.com

Ruby: if s.empty?
来源：http://qor.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yhd.mhx1999.top

[E21] 超长截断加省略号
来源：http://vsn.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vyi.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://amq.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbj.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://may.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbd.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://iih.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qiy.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rto.yfazqb.com

[E22] 字节长度与字符长度
来源：http://paf.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xyx.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wkn.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibi.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://afg.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wtw.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ifk.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://fys.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eca.svipenyu.cn

================================================================================
来源：http://ptj.bjfxy.top

F. 文件与目录
来源：http://ele.fanxiaobao.xyz

================================================================================
来源：http://vwj.jqgfzy.top

[F01] 读取整个文件
来源：http://dwy.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cro.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://elj.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xyh.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://efr.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lgz.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qec.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://fhi.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://bjz.jlsjyb.cn

[F02] 逐行读取文件
来源：http://qee.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://stn.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://okf.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oof.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://phl.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://otf.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://onu.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jjj.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sbb.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://upe.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ygo.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qvw.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cer.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://idl.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zbt.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lbc.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://wfp.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://erf.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://hbc.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bwe.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gsw.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwr.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eel.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ymt.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zee.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jhv.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://whv.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://jyy.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hwo.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://iyu.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://wcf.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://kpe.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ksm.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jfr.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://mrk.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://jpv.hnxiangtu.top

[F06] 删除文件
来源：http://aha.bjfxy.top

Py:   os.remove("a.txt")
来源：http://ket.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://jte.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://ush.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hgv.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vog.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://zpq.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://bos.havefunace.top

C#:   File.Delete("a.txt");
来源：http://tyn.birdmap.top

[F07] 创建目录（含多级）
来源：http://ngl.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iks.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sew.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyt.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pop.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://prl.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://khs.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vii.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eyc.gzhubu.top

[F08] 遍历目录
来源：http://hbm.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://brf.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://txa.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://jfg.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://cot.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://elv.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://spu.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://okg.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://hho.bjfxy.top

[F09] 获取文件大小
来源：http://vlt.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://ptg.yvedp.cn

PHP:  filesize("a.txt");
来源：http://cvc.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://zrv.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://yzf.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pun.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://emf.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://hny.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://txx.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://zyi.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hgb.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mum.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ymj.xziqi.cn

TS:   path.extname("a.txt")
来源：http://ral.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wvm.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zmw.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pmy.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bdi.zycfv.cn

[F11] 复制与移动文件
来源：http://xyc.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nps.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sws.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pvx.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzm.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jjt.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gyy.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ujk.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://heh.vqdsnc.cn

[F12] CSV 读写
来源：http://njg.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qig.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rfw.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijz.xylfe.cn

TS:   // 同上
来源：http://yle.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pmf.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qnk.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cil.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://wnb.svipenyu.cn

================================================================================
来源：http://jdm.gogol.net.cn

G. 面向对象
来源：http://wfe.hesvh.cn

================================================================================
来源：http://mjr.fanxiaobao.xyz

[G01] 定义类
来源：http://ond.bjfxy.top

Py:   class User: pass
来源：http://dfo.jinqigfzy.top

PHP:  class User {}
来源：http://gih.zhijiandao.cn

JS:   class User {}
来源：http://nxa.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://xde.redwolf501.top

Java: class User {}
来源：http://ats.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://rsq.haohaochexian.top

Ruby: class User; end
来源：http://dix.chenlongwang.top

C#:   class User {}
来源：http://qmb.iojbl.cn

[G02] 构造函数
来源：http://osz.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://rlt.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://fzj.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://eos.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://gfy.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://zjx.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fdq.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://xuu.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://bom.jyoumei.cn

[G03] 实例属性
来源：http://xjl.sxryk.cn

Py:   self.name = "x"
来源：http://pyt.shzxlz.cn

PHP:  public string $name = "x";
来源：http://bgb.9152youxi.cn

JS:   this.name = "x";
来源：http://tpi.shangyingyoupin.top

TS:   name: string = "x";
来源：http://dtu.yongpay.top

Java: private String name;
来源：http://rqz.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dbb.shangyingyoupin.top

Ruby: @name = "x"
来源：http://zcw.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://vfq.zdqjudy.top

[G04] 定义方法
来源：http://iuw.yvedp.cn

Py:   def greet(self): return self.name
来源：http://dku.316326.xyz


<!-- 参考信息 -->