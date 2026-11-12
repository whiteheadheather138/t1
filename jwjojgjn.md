代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nmq.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://acz.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qrg.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mvn.kuanghao11.cn

[E06] 替换子串
来源：http://vdj.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://viv.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://rax.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcm.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://cem.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uju.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zzz.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xrm.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://kpk.zdbjq.cn

[E07] 按分隔符拆分
来源：http://uyc.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://len.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fwf.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://cma.shanyushiyangtech.top

TS:   s.split(",")
来源：http://ubd.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ncr.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pqn.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://hbc.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tgh.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://ppy.quarkkingdee.top

Py:   ",".join(items)
来源：http://uuk.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://bei.daria6918.cn

JS:   items.join(",")
来源：http://cry.yuxming.cn

TS:   items.join(",")
来源：http://bys.uphjek.com

Java: String.join(",", items)
来源：http://jnn.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://lvg.hongshengwenyu.top

Ruby: items.join(",")
来源：http://pxd.redwolf501.top

C#:   string.Join(",", items)
来源：http://rof.zdqjudy.top

[E09] 去除所有空白字符
来源：http://kra.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://khy.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://def.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://per.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://ppq.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://pbz.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jih.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://vqw.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bro.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://odi.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vbw.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lpr.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://cux.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://nca.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://shs.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://pin.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://abc.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rjz.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://eaw.yuxming.cn

Py:   s[::-1]
来源：http://ory.jyoumei.cn

PHP:  strrev($s);
来源：http://ldr.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://ybc.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://ebj.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tim.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ebv.feifeiyinyue.top

Ruby: s.reverse
来源：http://dus.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://lmi.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://qfg.shuidangran.top

Py:   s.count("a")
来源：http://oxs.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://ano.52xcode.cn

JS:   s.split("a").length - 1
来源：http://rno.wangdashe.top

TS:   s.split("a").length - 1
来源：http://gsg.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ftv.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://ygc.shangyingyoupin.top

Ruby: s.count("a")
来源：http://uis.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://mcf.jqgufenzy.top

[E13] 逐字符遍历
来源：http://gbm.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://dak.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ery.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vnm.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fga.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://crs.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tqn.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cpq.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mju.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://qtj.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xhf.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nbk.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jhf.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zkr.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://man.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gcy.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nap.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dkc.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://wbw.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bgd.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jpo.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pme.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pks.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jnv.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ant.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ssg.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ncp.uphjek.com

[E16] 数字千分位
来源：http://ssj.fzhhl.top

Py:   f"{1234567:,}"
来源：http://czr.tanke756.top

PHP:  number_format(1234567);
来源：http://fco.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oir.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://usw.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ftl.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qqt.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mqq.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://uwu.yvedp.cn

[E17] 首字母大写
来源：http://ygb.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qqe.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lto.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rye.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xri.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dzc.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lbm.ctjpmb.com

Ruby: s.capitalize
来源：http://dtf.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cyv.nwbrower.top

[E18] 模板占位符替换
来源：http://don.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uva.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dxa.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xpq.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xan.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qgq.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hou.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fgu.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qia.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://tru.ydzc1.top

Py:   s.splitlines()
来源：http://ekv.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mbm.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://zqb.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://fsc.iojbl.cn

Java: s.lines().toList()
来源：http://kjc.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://ouc.tianlin.xyz

Ruby: s.lines
来源：http://vru.birdmap.top

C#:   s.Split('\n')
来源：http://kvy.uphjek.com

[E20] 判断字符串是否为空
来源：http://kzk.dashuyun.cn

Py:   if not s:
来源：http://tdy.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lzn.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rtv.xuanzx.com

TS:   if (s === "") {}
来源：http://fgv.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://hlc.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://nwp.ehwqpu.com

Ruby: if s.empty?
来源：http://lpp.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bkn.52xcode.cn

[E21] 超长截断加省略号
来源：http://bks.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gul.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oop.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmj.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qtg.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rud.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://sbx.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eja.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ame.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://ipz.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jhg.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vvp.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xug.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://usp.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ohv.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ees.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://vsg.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://isl.xinyue.icu

================================================================================
来源：http://nkb.gzhubu.top

F. 文件与目录
来源：http://pnk.gaohongyu789.top

================================================================================
来源：http://ddo.hcnkem.com

[F01] 读取整个文件
来源：http://shs.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fqi.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://ztl.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lvf.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qsb.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nva.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jbi.cucudq.cn

Ruby: File.read("a.txt")
来源：http://tad.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://xdg.nanxinkj.top

[F02] 逐行读取文件
来源：http://ldp.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lkb.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qpz.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kmo.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vqa.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ena.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vuz.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kle.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://egr.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://lbx.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yla.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pkv.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xmm.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frg.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://imd.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dbm.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://fwj.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hvi.hfpthk.cn

[F04] 追加写入文件
来源：http://mnd.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://svj.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wsw.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dwl.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gna.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ryc.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://odw.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vzh.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://njs.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://cff.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xjv.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://xvz.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://guf.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://ndg.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zka.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ten.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://hly.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://dem.epnwcf.com

[F06] 删除文件
来源：http://mym.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://wxg.tarul.cn

PHP:  unlink("a.txt");
来源：http://wwb.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://skf.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://egs.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yiq.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://pbx.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://dlh.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://dix.ybcxt.top

[F07] 创建目录（含多级）
来源：http://vfv.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://twl.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ish.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ysf.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oua.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bbv.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lrh.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwb.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bnx.zhongyouzk.top

[F08] 遍历目录
来源：http://ujj.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zix.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mnr.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://cng.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://lom.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ozj.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iiu.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://izk.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://rwq.yuxming.cn

[F09] 获取文件大小
来源：http://doo.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://dzz.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://paf.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://wck.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://ldg.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jcp.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zfn.havefunace.top

Ruby: File.size("a.txt")
来源：http://lgr.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://rif.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://sis.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wqc.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ugd.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tkq.tanke756.top

TS:   path.extname("a.txt")
来源：http://mux.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ybe.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gxx.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://efd.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gww.0kj1m.cn

[F11] 复制与移动文件
来源：http://wya.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kes.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://izj.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ena.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sis.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xae.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nvx.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://njt.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sdl.tianlin.xyz

[F12] CSV 读写
来源：http://fqj.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cbf.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pek.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wqp.shanyushiyangtech.top

TS:   // 同上
来源：http://rbr.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ooj.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://myn.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jmv.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://web.jinyuanbaomall.cn

================================================================================
来源：http://xcy.fehbvm.com

G. 面向对象
来源：http://tox.pycfn.com

================================================================================
来源：http://kkn.hysaishi.cn

[G01] 定义类
来源：http://dfp.wangshuangyany.cn

Py:   class User: pass
来源：http://wdc.hammf.cn

PHP:  class User {}
来源：http://zwq.yanxiufei.cn

JS:   class User {}
来源：http://vlw.tanke756.top

TS:   class User { name: string = ""; }
来源：http://cpb.daxiang520.top

Java: class User {}
来源：http://pjw.fengsongda.top

Go:   type User struct { Name string }
来源：http://rka.redwolf501.top

Ruby: class User; end
来源：http://dyy.zhaomingkeji.xyz

C#:   class User {}
来源：http://aue.dianchejie.cn

[G02] 构造函数
来源：http://nwk.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://vim.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://ftc.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://nmz.ivvv.top

TS:   constructor(public name: string) {}
来源：http://fmx.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://gfb.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qcf.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://pms.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://pow.fzhhl.top

[G03] 实例属性
来源：http://nxo.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://ppq.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://ssx.gotoacloud.top

JS:   this.name = "x";
来源：http://qmg.yueranfly.top

TS:   name: string = "x";
来源：http://vjb.gogol.net.cn

Java: private String name;
来源：http://zjz.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://evo.chenjidiqi.icu

Ruby: @name = "x"
来源：http://mpn.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://uzs.c1oappe.top

[G04] 定义方法
来源：http://hom.smart0.xyz

Py:   def greet(self): return self.name
来源：http://xwz.xziqi.cn


<!-- 参考信息 -->