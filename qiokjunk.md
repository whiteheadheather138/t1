代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://qit.xuanzx.com

TS:   s.split(",")
来源：http://ufx.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://stp.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vqg.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://jlf.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ynl.fehbvm.com

[E08] 数组按分隔符合并
来源：http://flw.tanke756.top

Py:   ",".join(items)
来源：http://tqg.ybcxt.top

PHP:  implode(",", $items);
来源：http://anz.andypj.xyz

JS:   items.join(",")
来源：http://ceq.yanxiufei.cn

TS:   items.join(",")
来源：http://kiq.sysykeji.top

Java: String.join(",", items)
来源：http://nxu.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://xbz.ydjk.org.cn

Ruby: items.join(",")
来源：http://msw.sxryk.cn

C#:   string.Join(",", items)
来源：http://tkn.haohaochexian.top

[E09] 去除所有空白字符
来源：http://ntn.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zzd.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sqy.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://xwe.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://btc.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://czz.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gnv.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://tha.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ffx.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://ioj.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://opw.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rvj.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://seg.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://xww.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://yam.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://auc.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://akk.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fdh.wangdashe.top

[E11] 反转字符串
来源：http://cye.yangfankeji.com

Py:   s[::-1]
来源：http://tzf.zdbjq.cn

PHP:  strrev($s);
来源：http://xrm.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://ksr.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://mwr.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uix.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uuo.jqgfzy.top

Ruby: s.reverse
来源：http://uyv.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://drm.jianghu66.top

[E12] 统计某字符出现次数
来源：http://tiq.yongpay.top

Py:   s.count("a")
来源：http://rox.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://lhr.epnwcf.com

JS:   s.split("a").length - 1
来源：http://nra.shuidangran.top

TS:   s.split("a").length - 1
来源：http://igi.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rdr.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://pvo.zhijiandao.cn

Ruby: s.count("a")
来源：http://ugx.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://zaz.fehbvm.com

[E13] 逐字符遍历
来源：http://dzh.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://ovj.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rrf.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bpr.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wha.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kzr.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zlm.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ebv.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ksz.daria6918.cn

[E14] URL 编码与 Base64
来源：http://mnf.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://exh.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://drw.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://edc.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jgb.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tdr.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://loi.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fcg.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://shx.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://lab.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xkg.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zak.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kzd.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eis.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xyt.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fro.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://azy.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vga.jiagoushi.top

[E16] 数字千分位
来源：http://gik.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://wqd.cqqwz.cn

PHP:  number_format(1234567);
来源：http://zik.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lcc.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yyu.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zga.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kkb.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ymr.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://nmc.zhijiandao.cn

[E17] 首字母大写
来源：http://lic.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qwu.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ifg.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sgg.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://btg.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tan.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fdf.redwolf501.top

Ruby: s.capitalize
来源：http://rij.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bnv.cucudq.cn

[E18] 模板占位符替换
来源：http://gqx.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wjy.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qzm.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rko.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fmk.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gon.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hkl.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yqo.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jhk.hesvh.cn

[E19] 多行文本按行拆分
来源：http://jbe.bjfxy.top

Py:   s.splitlines()
来源：http://faa.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://thu.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://upd.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://gqb.yangfankeji.com

Java: s.lines().toList()
来源：http://xac.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://enq.dianchejie.cn

Ruby: s.lines
来源：http://vxz.chenzaomai.com

C#:   s.Split('\n')
来源：http://ttv.bbcook.cn

[E20] 判断字符串是否为空
来源：http://ugm.shanyushiyangkeji.top

Py:   if not s:
来源：http://nmu.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zlh.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://veg.jyoumei.cn

TS:   if (s === "") {}
来源：http://nny.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://gvy.zdqjudy.top

Go:   if s == "" {}
来源：http://wvl.cqqwz.cn

Ruby: if s.empty?
来源：http://lkz.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vls.bbcook.cn

[E21] 超长截断加省略号
来源：http://oko.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tbg.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jfv.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pir.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tlh.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ywg.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://frp.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://usu.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ywc.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://btf.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tqc.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucd.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fmp.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqx.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jpp.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://llz.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://thl.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://weq.yfazqb.com

================================================================================
来源：http://hal.fehbvm.com

F. 文件与目录
来源：http://kju.yj20258888.top

================================================================================
来源：http://iql.haohaochexian.top

[F01] 读取整个文件
来源：http://jya.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mml.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://vdk.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fln.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jtl.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://sxk.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kis.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://sus.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://meo.fehbvm.com

[F02] 逐行读取文件
来源：http://fds.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://loi.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kjq.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rla.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eei.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eis.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bzn.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tpo.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vpe.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://dqe.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://alj.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xxg.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aeu.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oku.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zlz.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hyh.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://jtf.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jbg.guowangkeji.top

[F04] 追加写入文件
来源：http://bwp.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cpr.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://axe.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qkb.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bnc.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zcq.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kaj.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iev.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ihk.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://avy.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jyy.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://snw.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://yak.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://zuh.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ufx.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pwn.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://tol.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://omv.gogol.net.cn

[F06] 删除文件
来源：http://bdt.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://lgm.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://qjw.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://lqj.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ayi.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ksr.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://djl.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://jut.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://lyt.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://njk.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nzw.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wqe.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uoy.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fsy.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://igc.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://neu.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqe.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://omt.hfpthk.cn

[F08] 遍历目录
来源：http://tsx.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rjh.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uzi.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://yef.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://eoq.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wnx.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jkk.iojbl.cn

Ruby: Dir.children("dir")
来源：http://oxi.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://orq.jqgfzy.top

[F09] 获取文件大小
来源：http://pji.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://hrl.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://iaz.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://jrh.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://sba.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qch.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rly.tanke756.top

Ruby: File.size("a.txt")
来源：http://red.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://ygn.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://ylk.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aua.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nke.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dxi.smart0.xyz

TS:   path.extname("a.txt")
来源：http://mxp.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zwe.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uef.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qnb.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nch.uphjek.com

[F11] 复制与移动文件
来源：http://xti.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pcg.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hwm.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ely.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xcu.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ogq.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://brz.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ccb.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://avb.daxiang520.top

[F12] CSV 读写
来源：http://qbe.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ibh.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rli.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pjd.feifeiyinyue.top

TS:   // 同上
来源：http://koq.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uht.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aks.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vbe.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qwu.meibo888.top

================================================================================
来源：http://mcn.fzhhl.top

G. 面向对象
来源：http://mda.nanxuanxn.top

================================================================================
来源：http://fii.iojbl.cn

[G01] 定义类
来源：http://vlm.uphjek.com

Py:   class User: pass
来源：http://ivr.guowangkeji.top

PHP:  class User {}
来源：http://kew.hywenlv.cn

JS:   class User {}
来源：http://egj.ivvv.top

TS:   class User { name: string = ""; }
来源：http://oqo.mhx1999.top

Java: class User {}
来源：http://lka.gogol.net.cn

Go:   type User struct { Name string }
来源：http://dzh.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://tmq.gaohongyu789.top

C#:   class User {}
来源：http://qgm.vehdjk.com

[G02] 构造函数
来源：http://qts.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://xnv.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://qmw.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://pwl.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://dqc.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://dps.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qli.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://knk.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://mps.snrcjt.cn

[G03] 实例属性
来源：http://zus.ctjpmb.com

Py:   self.name = "x"
来源：http://oye.yongpay.top

PHP:  public string $name = "x";
来源：http://hvn.ppjwa.cn

JS:   this.name = "x";
来源：http://uoh.hongshengwenyu.top

TS:   name: string = "x";
来源：http://uaf.guowangkeji.top

Java: private String name;
来源：http://snw.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fez.zhengqikj.top

Ruby: @name = "x"
来源：http://uaj.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://mnz.svipenyu.cn

[G04] 定义方法
来源：http://dfc.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://bon.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dge.andypj.xyz

JS:   greet() { return this.name; }
来源：http://msc.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://grg.epnwcf.com

Java: String greet() { return name; }
来源：http://lfx.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://djy.nwbrower.top

Ruby: def greet; @name; end
来源：http://tpm.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://hmc.mhx1999.top

[G05] 继承
来源：http://srh.wangdashe.top

Py:   class Admin(User): pass
来源：http://sdz.52xcode.cn

PHP:  class Admin extends User {}
来源：http://orc.chenlongwang.top

JS:   class Admin extends User {}
来源：http://hwm.zycfv.cn

TS:   class Admin extends User {}
来源：http://zgx.snrcjt.cn

Java: class Admin extends User {}
来源：http://erh.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wca.316326.xyz

Ruby: class Admin < User; end
来源：http://jmx.316326.xyz

C#:   class Admin : User {}
来源：http://vol.jqgfzy.top


<!-- 参考信息 -->