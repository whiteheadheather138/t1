代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yog.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yhm.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bpw.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ssh.zdbjq.cn

[E06] 替换子串
来源：http://wjs.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ixf.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://rah.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tyq.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://ynl.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lad.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tcx.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jus.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://uoc.yuanzhike.top

[E07] 按分隔符拆分
来源：http://cct.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mlb.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gxm.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tom.hesvh.cn

TS:   s.split(",")
来源：http://vdw.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://zyh.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oqa.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://tfl.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wwh.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://xfa.havefunace.top

Py:   ",".join(items)
来源：http://nmb.yvedp.cn

PHP:  implode(",", $items);
来源：http://klp.cucudq.cn

JS:   items.join(",")
来源：http://pii.sweek.top

TS:   items.join(",")
来源：http://nse.nanxinkj.top

Java: String.join(",", items)
来源：http://etu.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://ymv.jlsjyb.cn

Ruby: items.join(",")
来源：http://qia.hammf.cn

C#:   string.Join(",", items)
来源：http://nzn.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://fjz.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ekg.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vaa.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://jmz.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://gvl.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://vah.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yzy.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qcd.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wix.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://uvq.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tbj.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vaa.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://pny.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://qaf.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://hfc.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://wgt.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ncu.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jsy.cdnleiting.top

[E11] 反转字符串
来源：http://kux.yanxiufei.cn

Py:   s[::-1]
来源：http://dcr.yonumen.top

PHP:  strrev($s);
来源：http://vqj.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://fml.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://xig.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ntb.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gft.guowangkeji.top

Ruby: s.reverse
来源：http://lgm.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://okj.ybcxt.top

[E12] 统计某字符出现次数
来源：http://ekm.ctjpmb.com

Py:   s.count("a")
来源：http://fnv.cheryme.top

PHP:  substr_count($s, "a");
来源：http://gak.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://roj.cashguo.top

TS:   s.split("a").length - 1
来源：http://dfl.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gqn.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://vuv.c1oappe.top

Ruby: s.count("a")
来源：http://ivj.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://nel.quarkkingdee.top

[E13] 逐字符遍历
来源：http://ptc.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://hsq.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cux.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mfy.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tmk.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://doe.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yza.hysaishi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wpx.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kbs.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://wvx.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://geq.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zny.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gyo.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xzr.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vee.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wjd.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fso.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://asv.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://dta.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ywy.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://axu.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yjt.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mob.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ucy.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jtg.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jms.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ynp.ivvv.top

[E16] 数字千分位
来源：http://yqd.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://rnb.sysykeji.top

PHP:  number_format(1234567);
来源：http://oem.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nkd.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lfn.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jcx.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ggf.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dmu.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://olj.jianghu66.top

[E17] 首字母大写
来源：http://jyt.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://odk.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kuz.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://biz.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jzy.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kwo.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hvu.yj20258.top

Ruby: s.capitalize
来源：http://xlc.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hzk.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://tuj.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ayq.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://abj.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://anz.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pem.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ear.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cyc.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gci.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ddc.cucudq.cn

[E19] 多行文本按行拆分
来源：http://dem.pycfn.com

Py:   s.splitlines()
来源：http://equ.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://njd.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://beb.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://onl.fehbvm.com

Java: s.lines().toList()
来源：http://ctf.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://vhf.vqdsnc.cn

Ruby: s.lines
来源：http://bqa.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://ywe.daria6918.cn

[E20] 判断字符串是否为空
来源：http://rjf.tanke756.top

Py:   if not s:
来源：http://rgh.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jog.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfd.nwbrower.top

TS:   if (s === "") {}
来源：http://kat.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://zbw.zdbjq.cn

Go:   if s == "" {}
来源：http://yxp.aizwys.cn

Ruby: if s.empty?
来源：http://djt.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dlv.yangfankeji.com

[E21] 超长截断加省略号
来源：http://zbn.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cdh.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lbq.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vmu.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fui.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wlu.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://pcs.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fme.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mzm.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://gir.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zfx.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbt.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zgi.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sor.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aze.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lqr.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://etu.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nou.jinqigufen.top

================================================================================
来源：http://dca.gaohongyu789.top

F. 文件与目录
来源：http://cux.feifeiyinyue.top

================================================================================
来源：http://uet.yangfankeji.com

[F01] 读取整个文件
来源：http://rrd.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://woc.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://ygc.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jsq.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tch.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://hyu.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mcg.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://yec.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jnq.jinqigufen.top

[F02] 逐行读取文件
来源：http://bop.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ncw.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wwc.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xiu.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dko.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mwh.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dzl.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fhk.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mpa.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://qtd.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mwf.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pdv.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://snz.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tpw.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nkq.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cak.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://qlr.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lxh.ybcxt.top

[F04] 追加写入文件
来源：http://vin.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://usu.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hzz.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://paq.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cqq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bup.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ngt.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://soa.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xbc.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://ffr.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cek.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://aof.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://wji.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://ext.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lgq.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://avm.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://xgy.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://vvm.zhijiandao.cn

[F06] 删除文件
来源：http://aod.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://uly.yj20258888.top

PHP:  unlink("a.txt");
来源：http://due.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rrd.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://bcj.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fvb.hammf.cn

Go:   os.Remove("a.txt")
来源：http://aur.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://axp.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://qqe.vehdjk.com

[F07] 创建目录（含多级）
来源：http://ylx.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xlg.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://khf.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ljq.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zon.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cya.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sfm.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvl.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gtq.dianchejie.cn

[F08] 遍历目录
来源：http://sij.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://viz.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wwv.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://spb.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://hwx.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://prn.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rtw.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://bhm.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://lgg.hongshengwenyu.top

[F09] 获取文件大小
来源：http://cgi.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://hzx.yueranfly.top

PHP:  filesize("a.txt");
来源：http://hxy.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://fjh.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://rky.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://mxb.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lnr.sxryk.cn

Ruby: File.size("a.txt")
来源：http://wwm.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://cui.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://dmd.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vcl.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ivv.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bus.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://hkt.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aen.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uyd.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xdy.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lvv.tian-w.cn

[F11] 复制与移动文件
来源：http://fdr.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jqi.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ldh.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fql.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wig.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eax.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://shz.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qbj.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uhx.epnwcf.com

[F12] CSV 读写
来源：http://xjp.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zct.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pzv.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fkg.ybcxt.top

TS:   // 同上
来源：http://lur.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aps.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lar.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cjm.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://npt.tanke756.top

================================================================================
来源：http://rls.tianlin.xyz

G. 面向对象
来源：http://dqh.zhiwuduotai.top

================================================================================
来源：http://mhb.fengsongda.top

[G01] 定义类
来源：http://nsb.fengsongda.top

Py:   class User: pass
来源：http://aei.xuetiantiany.cn

PHP:  class User {}
来源：http://dkk.zhengqikj.top

JS:   class User {}
来源：http://cii.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://ljq.zhijiandao.cn

Java: class User {}
来源：http://iii.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://vzc.smart0.xyz

Ruby: class User; end
来源：http://iye.shuidangran.top

C#:   class User {}
来源：http://fwg.xziqi.cn

[G02] 构造函数
来源：http://apf.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://xoc.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://bgj.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://gnq.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://pjd.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://xfu.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ngl.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://xmo.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://don.316326.xyz

[G03] 实例属性
来源：http://bqp.aizwys.cn

Py:   self.name = "x"
来源：http://wpn.yongpay.top

PHP:  public string $name = "x";
来源：http://dlv.52xcode.cn

JS:   this.name = "x";
来源：http://wuf.cheryme.top

TS:   name: string = "x";
来源：http://ycm.yangfankeji.com

Java: private String name;
来源：http://wta.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://smx.dianchejie.cn

Ruby: @name = "x"
来源：http://ywd.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://ypy.gogol.net.cn

[G04] 定义方法
来源：http://cup.pycfn.com

Py:   def greet(self): return self.name
来源：http://dpl.chenjidiqi.icu


<!-- 参考信息 -->