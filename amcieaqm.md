代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tkl.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cfk.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nnw.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bsp.snrcjt.cn

[E06] 替换子串
来源：http://ssq.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yzr.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://sql.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bth.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://eom.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ehh.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://swq.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xwi.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://lkp.birdmap.top

[E07] 按分隔符拆分
来源：http://qhp.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rtl.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://huu.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fao.gzhubu.top

TS:   s.split(",")
来源：http://gid.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ase.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lzp.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://cvc.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qnd.uphjek.com

[E08] 数组按分隔符合并
来源：http://iyb.gzhubu.top

Py:   ",".join(items)
来源：http://nfu.tianlin.xyz

PHP:  implode(",", $items);
来源：http://qzq.xuetiantiany.cn

JS:   items.join(",")
来源：http://bqx.gaohongyu789.top

TS:   items.join(",")
来源：http://oww.yongpay.top

Java: String.join(",", items)
来源：http://pxf.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://kpc.zhongyouzk.top

Ruby: items.join(",")
来源：http://qdu.hfpthk.cn

C#:   string.Join(",", items)
来源：http://cky.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://oig.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://veo.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyp.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://mtb.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://rcd.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://yrb.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wgh.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bpc.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tex.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://gvh.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpr.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xsc.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://tuj.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://xzz.hammf.cn

Java: String.format("%03d", 7)
来源：http://zxg.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zok.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ukm.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pvb.pengpengdd.cyou

[E11] 反转字符串
来源：http://xxh.birdmap.top

Py:   s[::-1]
来源：http://yzu.yangfankeji.com

PHP:  strrev($s);
来源：http://zmm.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://iai.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://fsu.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://uun.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zwq.jinqigufen.top

Ruby: s.reverse
来源：http://jau.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lhu.sysykeji.top

[E12] 统计某字符出现次数
来源：http://efo.nwbrower.top

Py:   s.count("a")
来源：http://ulg.tanke756.top

PHP:  substr_count($s, "a");
来源：http://kci.epnwcf.com

JS:   s.split("a").length - 1
来源：http://hdz.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://fxy.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ypb.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://qsp.yongpay.top

Ruby: s.count("a")
来源：http://scy.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://hqj.hywenlv.cn

[E13] 逐字符遍历
来源：http://ouw.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://ymf.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jmd.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uyi.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mrn.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tec.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bbh.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mtr.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aei.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://duq.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ahc.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yhs.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ojd.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wql.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://crx.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lkl.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jhr.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uwk.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://xoz.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sjq.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://coz.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sug.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ofj.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kah.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jgc.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://otk.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bid.tanke756.top

[E16] 数字千分位
来源：http://vdc.yj20258.top

Py:   f"{1234567:,}"
来源：http://ohi.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://zes.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pnv.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rbl.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qng.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kiu.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qze.yj20258.top

C#:   1234567.ToString("N0")
来源：http://iig.vqdsnc.cn

[E17] 首字母大写
来源：http://osl.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ixy.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dck.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bch.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kad.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xzl.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bwr.ydjk.org.cn

Ruby: s.capitalize
来源：http://ini.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tlg.yongpay.top

[E18] 模板占位符替换
来源：http://xrk.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vua.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tii.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kbo.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dtn.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fuc.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://afu.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dqp.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lsk.vehdjk.com

[E19] 多行文本按行拆分
来源：http://ajl.chenlongwang.top

Py:   s.splitlines()
来源：http://yjw.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rpl.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://swa.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://vqo.jqgufenzy.top

Java: s.lines().toList()
来源：http://anl.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://dzk.jqgfzy.top

Ruby: s.lines
来源：http://enk.iojbl.cn

C#:   s.Split('\n')
来源：http://ifs.daxiang520.top

[E20] 判断字符串是否为空
来源：http://bop.quarkkingdee.top

Py:   if not s:
来源：http://yop.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://czr.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ckf.smart0.xyz

TS:   if (s === "") {}
来源：http://ajl.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://vvg.gotoacloud.top

Go:   if s == "" {}
来源：http://del.guannengcc.top

Ruby: if s.empty?
来源：http://qfi.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lol.yangfankeji.com

[E21] 超长截断加省略号
来源：http://liq.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lcp.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cnc.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iyi.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxj.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gvn.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://jvm.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xci.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bgr.jianghu66.top

[E22] 字节长度与字符长度
来源：http://cdi.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zai.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iaj.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dze.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tfm.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bif.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://riv.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://xpj.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zwd.yanxiufei.cn

================================================================================
来源：http://szj.hcnkem.com

F. 文件与目录
来源：http://osa.yj202588.top

================================================================================
来源：http://pkl.hnqzz.top

[F01] 读取整个文件
来源：http://dzs.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nfn.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://gys.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://phu.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gpl.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jus.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tqo.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://qjx.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://hjj.jiagoushi.top

[F02] 逐行读取文件
来源：http://pqy.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ouy.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sgu.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kui.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://msa.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bnj.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zkp.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sgt.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ixb.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://dop.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bzq.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fte.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyo.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsi.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jkc.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tdy.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://kgj.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oyl.tian-w.cn

[F04] 追加写入文件
来源：http://odq.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fgr.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rtf.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rxu.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oty.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://acf.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jwq.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rgn.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yin.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://ixh.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://avp.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://gzs.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://zca.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://nai.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kkd.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jje.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://aer.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://qhv.ywan-chungtsiang.top

[F06] 删除文件
来源：http://ffo.yj202588.top

Py:   os.remove("a.txt")
来源：http://acc.tarul.cn

PHP:  unlink("a.txt");
来源：http://tgi.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://ovb.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kuq.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oco.shangyingyoupin.top

Go:   os.Remove("a.txt")
来源：http://vqc.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://swp.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://eue.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://poq.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://utg.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aou.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jpv.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zyw.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hra.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sxw.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pnr.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xhm.0kj1m.cn

[F08] 遍历目录
来源：http://msd.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://akq.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bel.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://hcd.xziqi.cn

TS:   fs.readdirSync("dir")
来源：http://gfk.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hxo.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bvk.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://xip.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://ouh.haohaochexian.top

[F09] 获取文件大小
来源：http://ylo.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://ctf.xuanzx.com

PHP:  filesize("a.txt");
来源：http://gwy.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://jrk.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://esa.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xra.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rqe.yonumen.top

Ruby: File.size("a.txt")
来源：http://xmp.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://tuy.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://oib.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdf.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hfn.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ggh.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://rdc.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wxx.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gvn.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://klw.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kyp.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://uxu.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mkp.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://owj.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbi.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cdm.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sts.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lpj.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://szi.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sjy.sysykeji.top

[F12] CSV 读写
来源：http://aaz.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pgd.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wco.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kvh.zhongyouzk.top

TS:   // 同上
来源：http://gtx.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qtg.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rvb.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pof.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://qzw.9152youxi.cn

================================================================================
来源：http://glh.ydzc1.top

G. 面向对象
来源：http://gbi.quarkkingdee.top

================================================================================
来源：http://mjv.xziqi.cn

[G01] 定义类
来源：http://bpv.tarul.cn

Py:   class User: pass
来源：http://vxb.sweek.top

PHP:  class User {}
来源：http://nat.tianlin.xyz

JS:   class User {}
来源：http://lus.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://cuo.fzhhl.top

Java: class User {}
来源：http://jft.yfazqb.com

Go:   type User struct { Name string }
来源：http://dih.gaohongyu789.top

Ruby: class User; end
来源：http://kaq.xylfe.cn

C#:   class User {}
来源：http://evj.sweek.top

[G02] 构造函数
来源：http://wwh.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://arr.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://efu.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://qmy.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://kgu.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://azv.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bps.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://dfb.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://smx.yuanzhike.top

[G03] 实例属性
来源：http://uwu.ivvv.top

Py:   self.name = "x"
来源：http://lfw.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://klg.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://sol.hnxiangtu.top

TS:   name: string = "x";
来源：http://yin.hnqzz.top

Java: private String name;
来源：http://fnf.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lei.9152youxi.cn

Ruby: @name = "x"
来源：http://mxr.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://esu.gaohongyu789.top

[G04] 定义方法
来源：http://lak.gzhubu.top

Py:   def greet(self): return self.name
来源：http://qyu.havefunace.top


<!-- 参考信息 -->