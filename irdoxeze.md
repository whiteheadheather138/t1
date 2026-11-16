代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://syl.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rmc.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qui.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://stc.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://lxh.uphjek.com

[E07] 按分隔符拆分
来源：http://rww.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://khz.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ibi.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oco.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://bmd.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://jhe.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvn.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://pkr.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nqf.cheryme.top

[E08] 数组按分隔符合并
来源：http://bvv.shangyingyoupin.top

Py:   ",".join(items)
来源：http://jaq.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://fst.kuanghao11.cn

JS:   items.join(",")
来源：http://cdr.hysaishi.cn

TS:   items.join(",")
来源：http://nlv.epnwcf.com

Java: String.join(",", items)
来源：http://vjz.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://vpw.xziqi.cn

Ruby: items.join(",")
来源：http://gzp.yonumen.top

C#:   string.Join(",", items)
来源：http://gxe.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://twk.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pdq.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fmo.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://ssa.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://lrb.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://goa.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rqc.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://typ.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yit.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://tzp.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fck.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ibe.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://qay.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://enr.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://mue.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aaf.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cwh.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rfm.xuanzx.com

[E11] 反转字符串
来源：http://krb.zycfv.cn

Py:   s[::-1]
来源：http://pgp.yonumen.top

PHP:  strrev($s);
来源：http://nkv.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://pyl.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://yaq.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://imf.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jnv.svipenyu.cn

Ruby: s.reverse
来源：http://zjj.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://bwp.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://foc.yangfankeji.com

Py:   s.count("a")
来源：http://twr.yj202588.top

PHP:  substr_count($s, "a");
来源：http://lza.yuxming.cn

JS:   s.split("a").length - 1
来源：http://pyb.xuanzx.com

TS:   s.split("a").length - 1
来源：http://tvv.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dou.cheryme.top

Go:   strings.Count(s, "a")
来源：http://alq.smart0.xyz

Ruby: s.count("a")
来源：http://iay.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://nwi.hesvh.cn

[E13] 逐字符遍历
来源：http://dok.birdmap.top

Py:   for ch in s: print(ch)
来源：http://agp.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://elr.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://pkt.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://rxk.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fcc.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uls.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oaf.tian-w.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aoj.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://lhi.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kfp.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ckz.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://buk.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hnk.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://etf.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cjw.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yav.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zgi.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://kcb.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://czq.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zjz.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vdt.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cfd.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mpw.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://odo.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qbl.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pvp.shzxlz.cn

[E16] 数字千分位
来源：http://voa.tian-w.cn

Py:   f"{1234567:,}"
来源：http://thx.yangfankeji.com

PHP:  number_format(1234567);
来源：http://oex.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gdn.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hgf.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bge.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lpx.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jzi.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://vyu.cashguo.top

[E17] 首字母大写
来源：http://iuz.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbf.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lyo.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbr.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfx.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ugn.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://waf.gaohongyu789.top

Ruby: s.capitalize
来源：http://xtx.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bjw.xylfe.cn

[E18] 模板占位符替换
来源：http://jnw.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mob.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xlw.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zat.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://afd.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ivp.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dai.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zem.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://opg.fengsongda.top

[E19] 多行文本按行拆分
来源：http://tej.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://mcz.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://arx.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://vlu.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://kxd.uphjek.com

Java: s.lines().toList()
来源：http://kps.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://pmf.shanyushiyangtech.top

Ruby: s.lines
来源：http://bpg.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://qvk.hesvh.cn

[E20] 判断字符串是否为空
来源：http://rcy.jinyuanbaomall.cn

Py:   if not s:
来源：http://onk.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bkp.jinghuilouyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfg.cucudq.cn

TS:   if (s === "") {}
来源：http://usz.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://pbg.hongshengwenyu.top

Go:   if s == "" {}
来源：http://vae.jyoumei.cn

Ruby: if s.empty?
来源：http://pbv.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ugf.yuanzhike.top

[E21] 超长截断加省略号
来源：http://ddp.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cxd.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://glo.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ion.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tpa.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jmj.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://bwg.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xls.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jgu.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://zvl.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://exb.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jvd.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ptl.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://swd.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sjn.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bnz.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://hon.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vkq.havefunace.top

================================================================================
来源：http://dhj.dianchejie.cn

F. 文件与目录
来源：http://rll.sxryk.cn

================================================================================
来源：http://hvk.yuanzhike.top

[F01] 读取整个文件
来源：http://zit.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xiw.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://vdx.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wsy.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvq.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mqh.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uov.xinyue.icu

Ruby: File.read("a.txt")
来源：http://uyh.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://nuz.daria6918.cn

[F02] 逐行读取文件
来源：http://ryy.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vle.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fct.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jrb.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opi.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uoj.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tvl.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://npo.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hlo.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://pat.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lhe.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yfg.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gns.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kzl.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://evu.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://idq.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://kvk.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iax.zhoulong.xyz

[F04] 追加写入文件
来源：http://ewg.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://llv.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bie.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oil.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eck.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hbb.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qsf.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uyo.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oqd.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://mtz.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zjr.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://gvg.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://pwp.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://cis.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://dxx.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rmt.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://gas.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://hdz.yongpay.top

[F06] 删除文件
来源：http://qoc.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://dgx.fengsongda.top

PHP:  unlink("a.txt");
来源：http://gtr.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://xgf.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://vye.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yep.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://emo.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://bpj.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://uxa.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://kes.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vsn.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sjp.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjb.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qmc.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tik.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bep.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fen.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zql.ctjpmb.com

[F08] 遍历目录
来源：http://erc.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ths.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sve.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://rxv.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://gcd.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ojw.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cug.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://qui.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://ehb.hnqzz.top

[F09] 获取文件大小
来源：http://eqj.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://otl.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://pdz.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://mkr.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://tpm.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://oel.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yxn.meibo888.top

Ruby: File.size("a.txt")
来源：http://tgo.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://phy.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://nvp.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ase.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://joj.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jsp.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://xvl.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dsh.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bqy.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rll.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sip.havefunace.top

[F11] 复制与移动文件
来源：http://twc.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qow.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qhn.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ptt.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jkd.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mdt.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lbq.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xfc.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zqz.zycfv.cn

[F12] CSV 读写
来源：http://zzr.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mwt.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bbk.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://guf.jinghuilouyu.cn

TS:   // 同上
来源：http://isi.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ijt.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vgc.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gur.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://fxd.zhongyouzk.top

================================================================================
来源：http://isf.52xcode.cn

G. 面向对象
来源：http://xzg.fengsongda.top

================================================================================
来源：http://mth.yuanzhike.top

[G01] 定义类
来源：http://yzz.zhiwuduotai.top

Py:   class User: pass
来源：http://tgh.sufxvd.cn

PHP:  class User {}
来源：http://ywk.guowangkeji.top

JS:   class User {}
来源：http://zdp.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://wev.bjfxy.top

Java: class User {}
来源：http://rul.fehbvm.com

Go:   type User struct { Name string }
来源：http://rmg.hcnkem.com

Ruby: class User; end
来源：http://jvi.dashuyun.cn

C#:   class User {}
来源：http://gpu.jlsjyb.cn

[G02] 构造函数
来源：http://goj.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://bbk.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://tqe.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://olp.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://hrl.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://izv.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yoz.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://mde.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://ymr.hesvh.cn

[G03] 实例属性
来源：http://oqu.guannengcc.top

Py:   self.name = "x"
来源：http://htk.mhx1999.top

PHP:  public string $name = "x";
来源：http://uui.wangshuangyany.cn

JS:   this.name = "x";
来源：http://dzj.shzxlz.cn

TS:   name: string = "x";
来源：http://nnm.hywenlv.cn

Java: private String name;
来源：http://qpe.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ykx.cdnleiting.top

Ruby: @name = "x"
来源：http://wlh.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://spp.jinqigufen.top

[G04] 定义方法
来源：http://fgi.meibo888.top

Py:   def greet(self): return self.name
来源：http://mnt.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lae.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://ojw.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://ivg.cheryme.top

Java: String greet() { return name; }
来源：http://rrm.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dpm.chenlongwang.top

Ruby: def greet; @name; end
来源：http://yko.daxiang520.top

C#:   public string Greet() => Name;
来源：http://wai.quarkkingdee.top

[G05] 继承
来源：http://bgp.tarul.cn


<!-- 参考信息 -->