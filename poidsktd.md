代发 wailian999

[E06] 替换子串
来源：http://snw.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iwo.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://hmr.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hkv.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://uhx.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqf.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eek.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xws.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://atk.cashguo.top

[E07] 按分隔符拆分
来源：http://ywk.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cde.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jmj.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oej.0kj1m.cn

TS:   s.split(",")
来源：http://avl.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://gsy.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gee.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://rxq.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://egw.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://aqh.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://nqp.zdbjq.cn

PHP:  implode(",", $items);
来源：http://yzl.fengsongda.top

JS:   items.join(",")
来源：http://vbx.snrcjt.cn

TS:   items.join(",")
来源：http://xll.shzxlz.cn

Java: String.join(",", items)
来源：http://fog.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://kxl.jianghu66.top

Ruby: items.join(",")
来源：http://qxh.pycfn.com

C#:   string.Join(",", items)
来源：http://xef.ivvv.top

[E09] 去除所有空白字符
来源：http://uua.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kwv.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://udw.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://yuk.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://zxm.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://buj.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yud.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://qcv.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xhj.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://hsn.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vve.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qax.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://fsx.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://jhr.zycfv.cn

Java: String.format("%03d", 7)
来源：http://jxj.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wwz.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yzm.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pdy.kuanghao11.cn

[E11] 反转字符串
来源：http://vab.cashguo.top

Py:   s[::-1]
来源：http://zbn.jinqigufen.top

PHP:  strrev($s);
来源：http://jjm.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://nhz.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://jje.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zgr.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxo.smart0.xyz

Ruby: s.reverse
来源：http://suc.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://edz.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://hiq.jinqigufen.top

Py:   s.count("a")
来源：http://ccz.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://ebn.birdmap.top

JS:   s.split("a").length - 1
来源：http://hhd.fzhhl.top

TS:   s.split("a").length - 1
来源：http://nel.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qdk.yj20258.top

Go:   strings.Count(s, "a")
来源：http://lbo.tianlin.xyz

Ruby: s.count("a")
来源：http://eyl.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://ilx.ivvv.top

[E13] 逐字符遍历
来源：http://bel.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://pvc.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://row.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://szc.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ffo.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ors.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://die.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qid.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ula.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://hfx.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://egs.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://esv.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pef.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jsq.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://idg.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bcb.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lmb.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://txj.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://brn.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tkg.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yzw.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uzf.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jlv.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zrr.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sqc.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ejr.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hfr.cqqwz.cn

[E16] 数字千分位
来源：http://yyh.yvedp.cn

Py:   f"{1234567:,}"
来源：http://cya.hesvh.cn

PHP:  number_format(1234567);
来源：http://lxl.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ixg.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bon.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cbb.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hix.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qzy.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://hiu.nanxinkj.top

[E17] 首字母大写
来源：http://vuy.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://avq.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ayw.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tdk.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sqs.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qmq.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fpx.gogol.net.cn

Ruby: s.capitalize
来源：http://gzw.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zpo.aibaodan.cn

[E18] 模板占位符替换
来源：http://wlg.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jbg.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mec.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://gpg.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://erg.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ipc.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zle.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kaz.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://srg.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://cnx.jqgfzy.top

Py:   s.splitlines()
来源：http://jar.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tgx.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://caf.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://vdk.snrcjt.cn

Java: s.lines().toList()
来源：http://qbz.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://pmo.hongshengwenyu.top

Ruby: s.lines
来源：http://wrn.sufxvd.cn

C#:   s.Split('\n')
来源：http://wzn.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://cnk.tarul.cn

Py:   if not s:
来源：http://kig.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ser.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hti.shzxlz.cn

TS:   if (s === "") {}
来源：http://ijv.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://zvw.yvedp.cn

Go:   if s == "" {}
来源：http://jax.yvedp.cn

Ruby: if s.empty?
来源：http://nrc.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ojs.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://dpx.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rrj.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uhl.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pxm.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fbo.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oyu.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://qxp.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rat.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kah.ybcxt.top

[E22] 字节长度与字符长度
来源：http://fuc.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fgp.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytp.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hiw.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wrq.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gro.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gns.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://bde.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lmx.sufxvd.cn

================================================================================
来源：http://dsf.feifeiyinyue.top

F. 文件与目录
来源：http://fpg.smart0.xyz

================================================================================
来源：http://rue.316326.xyz

[F01] 读取整个文件
来源：http://sia.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://huz.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://lka.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://okg.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gqy.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://umw.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqn.daxiang520.top

Ruby: File.read("a.txt")
来源：http://qug.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://ffs.gaohongyu789.top

[F02] 逐行读取文件
来源：http://gia.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nwn.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wrx.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vly.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://esc.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vwt.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ruf.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ajh.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jts.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://hjw.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mwe.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zlw.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sqw.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxc.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ubt.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mbj.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://mtx.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://odg.uphjek.com

[F04] 追加写入文件
来源：http://lpv.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zml.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wyj.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifx.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ich.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fcx.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yxi.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vsl.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pfb.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://dfu.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wsc.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://mps.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://kuh.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://cax.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mzm.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kop.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://yhm.birdmap.top

C#:   File.Exists("a.txt")
来源：http://obr.jinqigfzy.top

[F06] 删除文件
来源：http://zrh.uphjek.com

Py:   os.remove("a.txt")
来源：http://xsr.redwolf501.top

PHP:  unlink("a.txt");
来源：http://aeg.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://gxk.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://hsf.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eic.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://mis.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://bpj.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://hkm.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://ilp.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vsm.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ijf.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dty.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hxv.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dnh.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nst.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yxp.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cwx.bbcook.cn

[F08] 遍历目录
来源：http://hqq.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lkw.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dsg.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://yqk.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://bnv.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jsr.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://llm.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://swe.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://ebx.pengpengdd.cyou

[F09] 获取文件大小
来源：http://gxl.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://lpt.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://ref.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://mqm.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://cif.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://rix.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qsq.yvedp.cn

Ruby: File.size("a.txt")
来源：http://owj.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://utz.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://gnx.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fhu.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lzi.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lpe.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://qgo.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xrk.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tcn.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mqi.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://com.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://tgx.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ttg.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://okh.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://omm.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwe.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://til.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ggb.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hvw.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://trd.fktsv.cn

[F12] CSV 读写
来源：http://aoi.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fej.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gmt.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fcz.nanxinkj.top

TS:   // 同上
来源：http://dzi.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nyd.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hsa.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nab.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://oef.zhaomingkeji.xyz

================================================================================
来源：http://hbn.jianghu66.top

G. 面向对象
来源：http://hbb.cucudq.cn

================================================================================
来源：http://msb.smart0.xyz

[G01] 定义类
来源：http://qvx.sxryk.cn

Py:   class User: pass
来源：http://zdz.bbcook.cn

PHP:  class User {}
来源：http://ayw.zdqjudy.top

JS:   class User {}
来源：http://siv.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://acg.birdmap.top

Java: class User {}
来源：http://uoh.ctjpmb.com

Go:   type User struct { Name string }
来源：http://trz.ydzc1.top

Ruby: class User; end
来源：http://wma.chenlongwang.top

C#:   class User {}
来源：http://mrx.aizwys.cn

[G02] 构造函数
来源：http://jnw.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://och.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://pdr.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://zdl.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://vnq.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://sah.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jgu.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://rvs.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://mlq.yj20258888.top

[G03] 实例属性
来源：http://pbo.dianchejie.cn

Py:   self.name = "x"
来源：http://afl.fktsv.cn

PHP:  public string $name = "x";
来源：http://yrq.zdqjudy.top

JS:   this.name = "x";
来源：http://sml.yuxming.cn

TS:   name: string = "x";
来源：http://qek.xziqi.cn

Java: private String name;
来源：http://qjw.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xjo.ybcxt.top

Ruby: @name = "x"
来源：http://tks.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lri.wangdashe.top

[G04] 定义方法
来源：http://mus.gzhubu.top

Py:   def greet(self): return self.name
来源：http://ffd.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tgk.redwolf501.top

JS:   greet() { return this.name; }
来源：http://xth.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://yjr.ehwqpu.com

Java: String greet() { return name; }
来源：http://ojq.yvedp.cn


<!-- 参考信息 -->