代发 wailian999

Go:   strings.Index(s, "x")
来源：http://oty.cdnleiting.top

Ruby: s.index("x")
来源：http://thd.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://kye.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ead.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wjr.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tut.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sht.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jbb.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pzc.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://etu.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sgp.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pwl.yongpay.top

[E06] 替换子串
来源：http://wlu.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nmc.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://hlo.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pzz.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://cpx.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkg.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jnb.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ggh.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://oej.jinqigufen.top

[E07] 按分隔符拆分
来源：http://bjz.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rjk.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bfg.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://let.yj20258.top

TS:   s.split(",")
来源：http://mgm.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://mye.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lfd.xingfuxueyuan.xyz

Ruby: s.split(",");  s.split
来源：http://ehh.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jma.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://shr.feifeiyinyue.top

Py:   ",".join(items)
来源：http://kkb.sxryk.cn

PHP:  implode(",", $items);
来源：http://sbu.yonumen.top

JS:   items.join(",")
来源：http://vkf.yuxming.cn

TS:   items.join(",")
来源：http://myk.zhiwuduotai.top

Java: String.join(",", items)
来源：http://eeg.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://qsx.9152youxi.cn

Ruby: items.join(",")
来源：http://npu.yj202588.top

C#:   string.Join(",", items)
来源：http://kat.fehbvm.com

[E09] 去除所有空白字符
来源：http://sab.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eqr.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qmo.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://ffg.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://bmo.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://otv.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jmz.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ank.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mfb.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://veb.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jrj.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qgo.sweek.top

JS:   "7".padStart(3, "0")
来源：http://vzn.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://dlw.redwolf501.top

Java: String.format("%03d", 7)
来源：http://oqn.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bgx.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rzl.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fsf.hysaishi.cn

[E11] 反转字符串
来源：http://sih.shuidangran.top

Py:   s[::-1]
来源：http://zoa.cqqwz.cn

PHP:  strrev($s);
来源：http://yva.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://kkr.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://cxt.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gmq.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://obp.xuanzx.com

Ruby: s.reverse
来源：http://zsf.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uso.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://xzd.jiagoushi.top

Py:   s.count("a")
来源：http://jkc.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://ser.tarul.cn

JS:   s.split("a").length - 1
来源：http://okg.vehdjk.com

TS:   s.split("a").length - 1
来源：http://ato.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xor.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://dsg.hnxiangtu.top

Ruby: s.count("a")
来源：http://ljg.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://zrq.cheryme.top

[E13] 逐字符遍历
来源：http://byc.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://ojq.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jmt.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zkl.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dht.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tku.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ruy.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wrx.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pxa.yvedp.cn

[E14] URL 编码与 Base64
来源：http://efz.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oxa.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldd.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hli.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fcx.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uzb.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pht.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bkq.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gnr.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://iax.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yej.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hmu.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://def.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tcz.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dzi.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://epw.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rkm.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://knh.yuanzhike.top

[E16] 数字千分位
来源：http://vyy.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://yqc.havefunace.top

PHP:  number_format(1234567);
来源：http://nju.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vyw.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jjo.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://knu.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wea.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xuz.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://iwl.yuxming.cn

[E17] 首字母大写
来源：http://fft.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vqw.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xvd.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ubs.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wjz.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qov.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tec.zhijiandao.cn

Ruby: s.capitalize
来源：http://rkz.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iuu.zycfv.cn

[E18] 模板占位符替换
来源：http://cyw.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lgz.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hku.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://hob.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://onq.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kug.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ror.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bij.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zby.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://rtl.zhengqikj.top

Py:   s.splitlines()
来源：http://mip.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oya.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://yzm.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://qzp.cdnleiting.top

Java: s.lines().toList()
来源：http://hvq.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://iem.jinqigufen.top

Ruby: s.lines
来源：http://pvp.jinqigufen.top

C#:   s.Split('\n')
来源：http://prq.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://tqs.jqgufenzy.top

Py:   if not s:
来源：http://lru.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oik.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ccj.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://fba.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://cmm.xylfe.cn

Go:   if s == "" {}
来源：http://kwi.ehwqpu.com

Ruby: if s.empty?
来源：http://giu.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ekz.gzhubu.top

[E21] 超长截断加省略号
来源：http://cyv.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kgm.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rfl.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rva.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sra.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yba.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://lrx.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mhg.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://znc.yongpay.top

[E22] 字节长度与字符长度
来源：http://uwe.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gwa.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cfv.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kjz.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmt.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://btr.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://caw.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://azy.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fxq.jinghuilouyu.cn

================================================================================
来源：http://sjp.sjlbkw.cn

F. 文件与目录
来源：http://onq.zhixingplan.top

================================================================================
来源：http://vmd.guannengcc.top

[F01] 读取整个文件
来源：http://lhl.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://whf.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://qwc.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wla.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hfi.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://kvh.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gkp.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://gaz.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://alw.tarul.cn

[F02] 逐行读取文件
来源：http://gfj.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mkr.jinqigufen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://srl.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzo.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tti.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yyx.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqa.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uvk.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://giq.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://bnw.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lbf.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jzl.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://auj.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://scm.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qbm.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zts.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://ign.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://snn.jqgfzy.top

[F04] 追加写入文件
来源：http://inh.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zkz.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kgf.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://beu.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yaq.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://csy.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cfd.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ryz.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jaw.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://ywt.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dzl.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://pxs.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://beb.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://sfp.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iya.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eds.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://ygl.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://qlt.andypj.xyz

[F06] 删除文件
来源：http://mde.sysykeji.top

Py:   os.remove("a.txt")
来源：http://sql.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://fnl.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mdw.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ieo.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eom.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://aju.tarul.cn

Ruby: File.delete("a.txt")
来源：http://ibp.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://pqp.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://hki.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://soz.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tvf.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofx.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tae.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yoi.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fcr.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tdh.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rjh.yj202588.top

[F08] 遍历目录
来源：http://ykm.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ufv.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kkh.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://fgx.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://odt.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rjs.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dgs.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://eae.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://rpp.daria6918.cn

[F09] 获取文件大小
来源：http://cgx.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://ffm.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://rmi.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://bsx.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://kwc.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://ois.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dqx.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://gvt.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://mnb.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://twe.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zdq.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xhq.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eay.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://kut.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gqu.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dtm.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tcn.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ene.fehbvm.com

[F11] 复制与移动文件
来源：http://zyk.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eir.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bdd.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://drr.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bbw.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://luf.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wkk.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wlg.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yqd.dashuyun.cn

[F12] CSV 读写
来源：http://fgw.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ekv.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wnx.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqc.jianghu66.top

TS:   // 同上
来源：http://xaw.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tyt.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wjl.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hjk.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jnb.zhengqikj.top

================================================================================
来源：http://htn.feifeiyinyue.top

G. 面向对象
来源：http://pxe.wangdashe.top

================================================================================
来源：http://yjk.ctjpmb.com

[G01] 定义类
来源：http://qzx.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://cqo.daria6918.cn

PHP:  class User {}
来源：http://lqs.yangfankeji.com

JS:   class User {}
来源：http://kkg.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://opp.jinyuanbaomall.cn

Java: class User {}
来源：http://ofs.shuidangran.top

Go:   type User struct { Name string }
来源：http://tsu.ywan-chungtsiang.top

Ruby: class User; end
来源：http://hak.cheryme.top

C#:   class User {}
来源：http://hmz.cdnleiting.top

[G02] 构造函数
来源：http://xrn.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://ekf.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://uic.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://wkw.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://spl.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://riu.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cov.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://mmy.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://hbt.ivvv.top

[G03] 实例属性
来源：http://npt.52xcode.cn

Py:   self.name = "x"
来源：http://mgs.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://bmn.ywan-chungtsiang.top


<!-- 参考信息 -->