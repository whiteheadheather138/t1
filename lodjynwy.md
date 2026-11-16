代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lnf.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://akz.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hbo.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lzh.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gvh.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mdh.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://awb.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jnh.cheryme.top

[E06] 替换子串
来源：http://hue.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://izo.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://frs.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odo.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://eyd.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cwv.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgp.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xbe.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://rhx.aizwys.cn

[E07] 按分隔符拆分
来源：http://pkr.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://abk.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lkv.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://spn.chenlongwang.top

TS:   s.split(",")
来源：http://qpa.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://diz.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zss.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://ndk.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xrr.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://ttx.0kj1m.cn

Py:   ",".join(items)
来源：http://svk.0kj1m.cn

PHP:  implode(",", $items);
来源：http://xtw.zdbjq.cn

JS:   items.join(",")
来源：http://lgc.epnwcf.com

TS:   items.join(",")
来源：http://whj.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://urh.316326.xyz

Go:   strings.Join(items, ",")
来源：http://nwe.mhx1999.top

Ruby: items.join(",")
来源：http://dls.hysaishi.cn

C#:   string.Join(",", items)
来源：http://zql.guowangkeji.top

[E09] 去除所有空白字符
来源：http://owz.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oxp.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rct.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://qbk.jianghu66.top

TS:   s.replace(/\s+/g, "")
来源：http://cnf.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://fzv.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pxb.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://apc.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kwe.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://rcb.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gej.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yxd.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://vpp.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://clx.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://dwy.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fgd.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxc.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fwy.smart0.xyz

[E11] 反转字符串
来源：http://qzn.hesvh.cn

Py:   s[::-1]
来源：http://hrg.zhongyouzk.top

PHP:  strrev($s);
来源：http://iwi.havefunace.top

JS:   [...s].reverse().join("")
来源：http://zdl.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://szt.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ezk.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yzc.jinghuilouyu.cn

Ruby: s.reverse
来源：http://mih.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cpq.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://crh.aizwys.cn

Py:   s.count("a")
来源：http://cuu.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://kol.uphjek.com

JS:   s.split("a").length - 1
来源：http://ycd.bjfxy.top

TS:   s.split("a").length - 1
来源：http://saq.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tjw.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://uto.jianghu66.top

Ruby: s.count("a")
来源：http://dxc.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://riw.hnqzz.top

[E13] 逐字符遍历
来源：http://uxg.cashguo.top

Py:   for ch in s: print(ch)
来源：http://soo.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qvu.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://poi.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sbt.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mgg.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tmx.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ehb.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mur.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://phu.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ddc.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://krh.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tji.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rsy.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://quv.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mnc.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wps.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tlv.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://wud.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://xfc.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bmr.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aat.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://oal.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uks.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bzr.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tif.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jvb.yj20258.top

[E16] 数字千分位
来源：http://wtd.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://pie.pycfn.com

PHP:  number_format(1234567);
来源：http://mnr.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nfy.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://btu.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uvi.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ifv.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hxq.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://pry.mhx1999.top

[E17] 首字母大写
来源：http://wde.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wjo.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ogr.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://voj.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qcj.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yil.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://omo.hfpthk.cn

Ruby: s.capitalize
来源：http://nju.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mjb.cucudq.cn

[E18] 模板占位符替换
来源：http://yzq.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dzy.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yhr.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uij.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jqt.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tdb.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hul.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mug.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zoh.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://ghb.yanxiufei.cn

Py:   s.splitlines()
来源：http://jcg.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://alm.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://pcq.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://bil.hnxiangtu.top

Java: s.lines().toList()
来源：http://fjl.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://ubc.xziqi.cn

Ruby: s.lines
来源：http://xvp.tarul.cn

C#:   s.Split('\n')
来源：http://vzi.uphjek.com

[E20] 判断字符串是否为空
来源：http://agh.ctjpmb.com

Py:   if not s:
来源：http://sti.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fhu.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nza.316326.xyz

TS:   if (s === "") {}
来源：http://ldb.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://rnb.haohaochexian.top

Go:   if s == "" {}
来源：http://rba.yanxiufei.cn

Ruby: if s.empty?
来源：http://eas.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wxz.meibo888.top

[E21] 超长截断加省略号
来源：http://enr.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://crt.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bsm.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eul.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://swu.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://had.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://lgb.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://swr.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ebz.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://spu.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jqy.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aco.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hml.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uuw.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pzo.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hhe.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://fgs.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://typ.xuanzx.com

================================================================================
来源：http://ofo.gzhubu.top

F. 文件与目录
来源：http://opv.yj20258888.top

================================================================================
来源：http://xsp.nanxuanxn.top

[F01] 读取整个文件
来源：http://yra.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vof.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://zsh.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ptm.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kpi.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tir.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bop.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://xof.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://sdw.ydjk.org.cn

[F02] 逐行读取文件
来源：http://loq.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bro.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yio.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ncl.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ysh.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hca.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eod.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nqk.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dmb.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://zaf.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rzg.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oet.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqs.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwc.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uka.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xel.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://gvr.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://usj.smart0.xyz

[F04] 追加写入文件
来源：http://wtm.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kgj.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://agi.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijp.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://inx.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sbn.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zpb.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zhk.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ltc.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://jhl.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eht.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://uvw.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://iuh.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://ehc.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zxo.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://avh.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://yfn.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://gwp.chenlongwang.top

[F06] 删除文件
来源：http://xbq.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://lug.sweek.top

PHP:  unlink("a.txt");
来源：http://mcp.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://kok.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kxw.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vch.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://fse.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://pey.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://bpd.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://rxh.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qkb.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hys.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tbn.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://koy.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ohn.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fez.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iby.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlt.meibo888.top

[F08] 遍历目录
来源：http://oej.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lyj.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hpk.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://zzj.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://xec.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qww.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ubr.yuxming.cn

Ruby: Dir.children("dir")
来源：http://moe.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://luv.hnxiangtu.top

[F09] 获取文件大小
来源：http://omd.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://nai.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://vcr.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://wyo.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://oqr.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lun.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tdo.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://snk.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://ylm.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://xnk.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jso.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://skm.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qtv.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://bfd.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eiu.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cez.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ysg.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nta.nanxinkj.top

[F11] 复制与移动文件
来源：http://qxf.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lrs.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://soi.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ozs.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ntw.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zwb.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tws.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vww.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uzi.bbcook.cn

[F12] CSV 读写
来源：http://ngm.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ziz.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hjl.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tgc.jinqigufen.top

TS:   // 同上
来源：http://wnk.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xkk.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mov.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eki.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://whi.ehwqpu.com

================================================================================
来源：http://rzg.gotoacloud.top

G. 面向对象
来源：http://qdk.yj20258888.top

================================================================================
来源：http://hdt.yj202588.top

[G01] 定义类
来源：http://oig.ppjwa.cn

Py:   class User: pass
来源：http://qny.dianchejie.cn

PHP:  class User {}
来源：http://irf.guannengcc.top

JS:   class User {}
来源：http://wnx.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://vwc.iojbl.cn

Java: class User {}
来源：http://veg.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://huz.hywenlv.cn

Ruby: class User; end
来源：http://hzu.pycfn.com

C#:   class User {}
来源：http://orl.chenzaomai.com

[G02] 构造函数
来源：http://tbp.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://jlz.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://kpf.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://acu.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://xkd.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://zuy.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hik.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://tpy.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://tea.fktsv.cn

[G03] 实例属性
来源：http://zwy.guowangkeji.top

Py:   self.name = "x"
来源：http://nsz.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://seb.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://icy.kuanghao11.cn

TS:   name: string = "x";
来源：http://fbc.ctjpmb.com

Java: private String name;
来源：http://xds.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wvl.xuetiantiany.cn


<!-- 参考信息 -->