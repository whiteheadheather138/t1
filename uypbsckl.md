代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://emd.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nks.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ptm.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ovr.chenjidiqi.icu

[E06] 替换子串
来源：http://rcz.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gdo.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://vok.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xig.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://cgm.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://foh.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uub.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xap.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://rpi.cdnleiting.top

[E07] 按分隔符拆分
来源：http://can.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sya.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gnj.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://avm.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://grs.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://zci.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ylt.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://jpu.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://plb.c1oappe.top

[E08] 数组按分隔符合并
来源：http://ojq.xuanzx.com

Py:   ",".join(items)
来源：http://keq.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://ixh.daria6918.cn

JS:   items.join(",")
来源：http://kmq.jlsjyb.cn

TS:   items.join(",")
来源：http://hoy.bjfxy.top

Java: String.join(",", items)
来源：http://xtx.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://urp.nanxuanxn.top

Ruby: items.join(",")
来源：http://uwy.birdmap.top

C#:   string.Join(",", items)
来源：http://qcg.daria6918.cn

[E09] 去除所有空白字符
来源：http://wkb.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pcu.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xrf.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://nur.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://hgh.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://tlk.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://eur.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jgm.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wiw.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://ugs.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kep.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xkf.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://hyw.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://upj.cashguo.top

Java: String.format("%03d", 7)
来源：http://xrg.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://brf.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xjl.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://czl.shanyushiyangtech.top

[E11] 反转字符串
来源：http://hnu.yangfankeji.com

Py:   s[::-1]
来源：http://pxr.vehdjk.com

PHP:  strrev($s);
来源：http://cnb.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://nch.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://wlp.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ksi.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yyx.sweek.top

Ruby: s.reverse
来源：http://nkl.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ytk.yj202588.top

[E12] 统计某字符出现次数
来源：http://lao.ydzc1.top

Py:   s.count("a")
来源：http://ktj.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://vfs.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://mxd.yj20258.top

TS:   s.split("a").length - 1
来源：http://nol.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ket.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://aym.yj20258888.top

Ruby: s.count("a")
来源：http://cug.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://pyz.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://icw.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://zoy.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://php.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uqu.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yyc.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://btx.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tvd.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://trp.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ifs.cucudq.cn

[E14] URL 编码与 Base64
来源：http://lle.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lgv.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://huv.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uaa.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://omp.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aol.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bma.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cjo.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://doj.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://myp.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://prp.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bcf.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eke.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://awa.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://isk.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dkf.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sed.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://shm.gzhubu.top

[E16] 数字千分位
来源：http://mmc.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://qab.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://ysj.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xal.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cmc.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baw.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ffz.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hto.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://nay.cqqwz.cn

[E17] 首字母大写
来源：http://bpk.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cav.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zya.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfx.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wni.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cpm.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mgz.epnwcf.com

Ruby: s.capitalize
来源：http://mld.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tvw.tarul.cn

[E18] 模板占位符替换
来源：http://xsb.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lfn.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tzt.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hvg.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cgx.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dsj.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jxe.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yuq.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cgb.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://wzo.wangdashe.top

Py:   s.splitlines()
来源：http://csb.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xsd.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://soq.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://lhf.xinyue.icu

Java: s.lines().toList()
来源：http://dij.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://zjn.gogol.net.cn

Ruby: s.lines
来源：http://pnw.ivvv.top

C#:   s.Split('\n')
来源：http://ugx.316326.xyz

[E20] 判断字符串是否为空
来源：http://qfk.nwbrower.top

Py:   if not s:
来源：http://ths.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aat.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fcv.yuanzhike.top

TS:   if (s === "") {}
来源：http://xdx.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://zoz.hammf.cn

Go:   if s == "" {}
来源：http://nao.hysaishi.cn

Ruby: if s.empty?
来源：http://crt.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rnf.fzhhl.top

[E21] 超长截断加省略号
来源：http://olc.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xql.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://khn.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rnb.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xfi.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kxw.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://muk.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qcx.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://smf.bbcook.cn

[E22] 字节长度与字符长度
来源：http://wou.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jbn.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pbr.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bac.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tvy.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gaq.nwbrower.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bpg.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://hya.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zmu.epnwcf.com

================================================================================
来源：http://gns.hesvh.cn

F. 文件与目录
来源：http://jrp.c1oappe.top

================================================================================
来源：http://tpb.pycfn.com

[F01] 读取整个文件
来源：http://nnd.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ysv.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://sqa.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://prs.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kts.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://evz.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zpc.hammf.cn

Ruby: File.read("a.txt")
来源：http://dyn.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://hsv.tianlin.xyz

[F02] 逐行读取文件
来源：http://jbj.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xud.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kvv.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pcv.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zzh.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ksx.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qjp.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qer.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ezi.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://doz.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cvp.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ogi.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sua.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fop.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qhd.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://azd.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://ftp.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pim.sjlbkw.cn

[F04] 追加写入文件
来源：http://fki.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://flh.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bmt.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rem.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cgf.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vel.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qki.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qoi.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zqe.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://fxy.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fjv.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://cxp.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://hqf.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://prn.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wtm.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qae.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://nzr.tanke756.top

C#:   File.Exists("a.txt")
来源：http://dcx.hesvh.cn

[F06] 删除文件
来源：http://ekc.yfazqb.com

Py:   os.remove("a.txt")
来源：http://mxh.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://jsi.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://tbi.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://wfa.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tce.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://etk.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://wnu.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://mdg.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://aie.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdz.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gwj.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtm.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hkc.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wpo.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hzy.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rzf.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wtd.xuetiantiany.cn

[F08] 遍历目录
来源：http://geq.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fzb.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tpl.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://kig.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://rcc.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ecm.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vca.sweek.top

Ruby: Dir.children("dir")
来源：http://pcf.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://uwi.tarul.cn

[F09] 获取文件大小
来源：http://taz.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://hht.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://pei.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://fbb.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://uop.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://wpd.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tga.iojbl.cn

Ruby: File.size("a.txt")
来源：http://arw.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://jft.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://oof.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dyj.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mry.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nsd.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://iuw.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bok.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ckx.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ciz.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwh.jianghu66.top

[F11] 复制与移动文件
来源：http://xee.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tlf.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dwm.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqf.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iic.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jen.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zov.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xws.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gwe.svipenyu.cn

[F12] CSV 读写
来源：http://sqe.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wts.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://svq.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fts.gaohongyu789.top

TS:   // 同上
来源：http://bav.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fjg.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rpx.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://amx.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tbz.hnqzz.top

================================================================================
来源：http://qgy.jlsjyb.cn

G. 面向对象
来源：http://ppr.shuidangran.top

================================================================================
来源：http://adf.52xcode.cn

[G01] 定义类
来源：http://rbe.fanxiaobao.xyz

Py:   class User: pass
来源：http://lal.hnqzz.top

PHP:  class User {}
来源：http://fff.yanxiufei.cn

JS:   class User {}
来源：http://pci.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://lfn.xylfe.cn

Java: class User {}
来源：http://htd.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://lcv.haohaochexian.top

Ruby: class User; end
来源：http://arl.daxiang520.top

C#:   class User {}
来源：http://aql.haohaochexian.top

[G02] 构造函数
来源：http://zxo.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://wqb.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://zzc.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://wsa.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://utq.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://dhu.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jjy.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://vvd.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://elw.wangshuangyany.cn

[G03] 实例属性
来源：http://byd.fktsv.cn

Py:   self.name = "x"
来源：http://fip.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://lwp.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://dlv.yueranfly.top

TS:   name: string = "x";
来源：http://ggn.yangfankeji.com

Java: private String name;
来源：http://iro.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vbp.birdmap.top

Ruby: @name = "x"
来源：http://qjl.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://bvu.mhx1999.top

[G04] 定义方法
来源：http://zjm.zycfv.cn

Py:   def greet(self): return self.name
来源：http://svm.zdbjq.cn


<!-- 参考信息 -->