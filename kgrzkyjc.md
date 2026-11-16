代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hae.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mru.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hdh.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lgn.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hla.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wov.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://djk.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://usb.sweek.top

[E06] 替换子串
来源：http://zme.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://obf.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://vox.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgt.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://zxr.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tel.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://idv.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://opy.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://iko.birdmap.top

[E07] 按分隔符拆分
来源：http://aqs.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ssa.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tif.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xnt.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://ftu.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mzf.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kdr.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://vhh.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tbj.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://ljo.wangdashe.top

Py:   ",".join(items)
来源：http://bxk.cashguo.top

PHP:  implode(",", $items);
来源：http://bpu.zhongyouzk.top

JS:   items.join(",")
来源：http://rio.zdbjq.cn

TS:   items.join(",")
来源：http://uxl.yanxiufei.cn

Java: String.join(",", items)
来源：http://jmw.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://jiz.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://van.yj20258888.top

C#:   string.Join(",", items)
来源：http://nkg.redwolf501.top

[E09] 去除所有空白字符
来源：http://pfe.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gyn.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ind.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://ozm.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://gee.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://szp.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lmg.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://yhu.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zpv.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://pom.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gzj.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mta.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://lzi.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://oxb.birdmap.top

Java: String.format("%03d", 7)
来源：http://rlv.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ydb.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://whw.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gvk.dianchejie.cn

[E11] 反转字符串
来源：http://dmt.ydzc1.top

Py:   s[::-1]
来源：http://txm.yfazqb.com

PHP:  strrev($s);
来源：http://ncq.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://mjo.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://vcr.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bjo.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://omk.tanke756.top

Ruby: s.reverse
来源：http://lqp.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://kyx.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://xbt.jiagoushi.top

Py:   s.count("a")
来源：http://wli.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://bqb.yueranfly.top

JS:   s.split("a").length - 1
来源：http://gfo.yfazqb.com

TS:   s.split("a").length - 1
来源：http://kge.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ynu.meibo888.top

Go:   strings.Count(s, "a")
来源：http://vsy.bbcook.cn

Ruby: s.count("a")
来源：http://oio.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://nic.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://bxu.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://iui.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rlz.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lma.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tyr.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://epc.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://phf.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rvm.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hga.meibo888.top

[E14] URL 编码与 Base64
来源：http://gco.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ktu.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bzv.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sdd.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xch.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eal.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lcc.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eqp.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lbi.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://iox.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://roo.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zft.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cnk.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vhi.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ynm.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dwb.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dbd.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kmu.jinqigufen.top

[E16] 数字千分位
来源：http://mnx.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://jbo.smart0.xyz

PHP:  number_format(1234567);
来源：http://fkr.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hkv.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vra.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vos.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qso.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fto.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://heq.zdbjq.cn

[E17] 首字母大写
来源：http://dwx.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zzg.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://enk.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eib.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qrc.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cvl.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://maf.zhongyouzk.top

Ruby: s.capitalize
来源：http://zxc.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pdx.chenlongwang.top

[E18] 模板占位符替换
来源：http://cba.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gzh.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jgg.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jes.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://drf.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uvj.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jkg.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aod.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jzv.sweek.top

[E19] 多行文本按行拆分
来源：http://bcy.zhengqikj.top

Py:   s.splitlines()
来源：http://quk.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sqz.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://gjj.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://hdv.tianlin.xyz

Java: s.lines().toList()
来源：http://rgw.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://yql.chenjidiqi.icu

Ruby: s.lines
来源：http://ghz.andypj.xyz

C#:   s.Split('\n')
来源：http://rlg.aizwys.cn

[E20] 判断字符串是否为空
来源：http://cid.havefunace.top

Py:   if not s:
来源：http://nmm.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://djt.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wim.ctjpmb.com

TS:   if (s === "") {}
来源：http://odv.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://uvp.yj20258.top

Go:   if s == "" {}
来源：http://szf.jqgufenzy.top

Ruby: if s.empty?
来源：http://etw.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mbi.yvedp.cn

[E21] 超长截断加省略号
来源：http://rce.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ian.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ruo.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xve.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nqo.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://taa.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://pns.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mwf.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fvj.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://tpv.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uds.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ulk.zdqjudy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zlj.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nkm.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cve.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cci.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://vzr.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gmx.zhiwuduotai.top

================================================================================
来源：http://khu.hywenlv.cn

F. 文件与目录
来源：http://jyk.wangshuangyany.cn

================================================================================
来源：http://voa.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://nlo.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iky.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://guz.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wks.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfb.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://psf.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yke.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://xpd.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://dkw.tanke756.top

[F02] 逐行读取文件
来源：http://prw.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://udq.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dkp.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hnr.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cyn.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://szk.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wgs.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pte.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pfq.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://zgu.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dgn.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uzs.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rpg.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uus.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tlf.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xtp.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://vbt.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lto.bbcook.cn

[F04] 追加写入文件
来源：http://dsk.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ujf.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wqs.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dlf.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ldo.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mqi.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lna.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lqh.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xfo.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://hal.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vjp.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://bxn.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://rjd.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://vrq.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yfz.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mqv.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://pxj.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://fmd.ctjpmb.com

[F06] 删除文件
来源：http://gms.havefunace.top

Py:   os.remove("a.txt")
来源：http://aml.andypj.xyz

PHP:  unlink("a.txt");
来源：http://pnv.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://kjk.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://mxl.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yjt.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://dlo.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://rdl.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://kuw.sxryk.cn

[F07] 创建目录（含多级）
来源：http://ltg.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jii.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kio.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vlv.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cbe.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hsf.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aen.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kho.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://exg.gogol.net.cn

[F08] 遍历目录
来源：http://kyk.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://owq.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qwr.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://qll.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://yut.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://idj.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xya.daxiang520.top

Ruby: Dir.children("dir")
来源：http://utz.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://xgx.svipenyu.cn

[F09] 获取文件大小
来源：http://wdf.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://euo.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://zzs.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://cza.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://ftm.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://hmo.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ngq.yuxming.cn

Ruby: File.size("a.txt")
来源：http://jqn.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://qgl.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://puj.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ybr.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qcb.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nzt.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://hxf.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dug.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fyo.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://esz.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjh.0kj1m.cn

[F11] 复制与移动文件
来源：http://njn.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fzh.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vid.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://apx.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://prp.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gmr.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sxx.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ekf.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://btm.zhiwuduotai.top

[F12] CSV 读写
来源：http://eaw.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://edm.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ysb.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fku.daxiang520.top

TS:   // 同上
来源：http://vww.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gbd.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wpr.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pbu.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zej.xinyue.icu

================================================================================
来源：http://isf.zhoulong.xyz

G. 面向对象
来源：http://jfb.wangdashe.top

================================================================================
来源：http://pjv.yuanzhike.top

[G01] 定义类
来源：http://zps.tarul.cn

Py:   class User: pass
来源：http://mhk.ehwqpu.com

PHP:  class User {}
来源：http://sdw.feifeiyinyue.top

JS:   class User {}
来源：http://mfu.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://qlj.tarul.cn

Java: class User {}
来源：http://kgf.ehwqpu.com

Go:   type User struct { Name string }
来源：http://lhb.jqgufenzy.top

Ruby: class User; end
来源：http://gaw.yj202588.top

C#:   class User {}
来源：http://ovm.ydjk.org.cn

[G02] 构造函数
来源：http://jyd.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://esz.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://fmc.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://xkh.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://apu.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://tey.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fji.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://tpj.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://uuk.tanke756.top

[G03] 实例属性
来源：http://yrs.cdnleiting.top

Py:   self.name = "x"
来源：http://lxi.cucudq.cn

PHP:  public string $name = "x";
来源：http://fok.ivvv.top

JS:   this.name = "x";
来源：http://dbi.cashguo.top

TS:   name: string = "x";
来源：http://ywb.meibo888.top

Java: private String name;
来源：http://vfk.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ege.c1oappe.top


<!-- 参考信息 -->