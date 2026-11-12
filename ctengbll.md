代发 wailian999

Go:   strings.Index(s, "x")
来源：http://xnv.cqqwz.cn

Ruby: s.index("x")
来源：http://izg.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://zkr.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rnr.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itu.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cmz.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wfk.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wgq.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wda.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nkz.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hnn.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eku.daria6918.cn

[E06] 替换子串
来源：http://pjy.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://moa.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://nug.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fse.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://uor.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oro.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://buv.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hex.cheryme.top

C#:   s.Replace("a", "b")
来源：http://zjr.havefunace.top

[E07] 按分隔符拆分
来源：http://sfu.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qgx.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pnx.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qzk.yanxiufei.cn

TS:   s.split(",")
来源：http://sdn.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zxc.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwp.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://sca.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kwf.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://xgd.cheryme.top

Py:   ",".join(items)
来源：http://oye.yueranfly.top

PHP:  implode(",", $items);
来源：http://sxj.daria6918.cn

JS:   items.join(",")
来源：http://ddg.gzhubu.top

TS:   items.join(",")
来源：http://nwv.yonumen.top

Java: String.join(",", items)
来源：http://wcc.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://ssc.guowangkeji.top

Ruby: items.join(",")
来源：http://ccj.ctjpmb.com

C#:   string.Join(",", items)
来源：http://fkv.gotoacloud.top

[E09] 去除所有空白字符
来源：http://oym.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kdv.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ibz.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://pqj.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://rhp.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://jlr.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://jly.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mdz.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zbl.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://rvz.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://evg.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wsv.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://koi.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://efm.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://crb.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ojd.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rex.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fmi.uphjek.com

[E11] 反转字符串
来源：http://dym.aibaodan.cn

Py:   s[::-1]
来源：http://uxr.chenlongwang.top

PHP:  strrev($s);
来源：http://jlw.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://muy.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://tzl.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://obu.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aqw.hesvh.cn

Ruby: s.reverse
来源：http://oxj.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://gbm.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://xxt.shanyushiyangtech.top

Py:   s.count("a")
来源：http://xey.yj202588.top

PHP:  substr_count($s, "a");
来源：http://kgk.yj20258.top

JS:   s.split("a").length - 1
来源：http://avd.ydzc1.top

TS:   s.split("a").length - 1
来源：http://zgy.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kos.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://ugz.hywenlv.cn

Ruby: s.count("a")
来源：http://tse.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://jdx.yueranfly.top

[E13] 逐字符遍历
来源：http://iiw.havefunace.top

Py:   for ch in s: print(ch)
来源：http://hts.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fgv.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wyh.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://upy.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://llt.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vym.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rfk.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://odu.ydzc1.top

[E14] URL 编码与 Base64
来源：http://djd.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nqp.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qmd.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dvw.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://daz.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hsp.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zxl.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://frg.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qeb.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://qkd.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zqk.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cwx.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kdj.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ihq.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vkz.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xyk.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fvk.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yjw.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://xex.hcnkem.com

Py:   f"{1234567:,}"
来源：http://wnv.pycfn.com

PHP:  number_format(1234567);
来源：http://pxf.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tsk.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ren.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://adf.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ddq.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kyh.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://eji.nanxinkj.top

[E17] 首字母大写
来源：http://gyh.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chh.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fpk.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xba.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dkk.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bdh.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kza.cucudq.cn

Ruby: s.capitalize
来源：http://vid.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ctz.andypj.xyz

[E18] 模板占位符替换
来源：http://zyu.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wvz.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzq.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eeh.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iyr.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bwg.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fld.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hcv.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mma.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://lzv.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://rek.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eul.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://jyl.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://bjk.sysykeji.top

Java: s.lines().toList()
来源：http://epm.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://nmq.mhx1999.top

Ruby: s.lines
来源：http://hmu.guannengcc.top

C#:   s.Split('\n')
来源：http://uqi.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://yyv.mhx1999.top

Py:   if not s:
来源：http://xmb.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ruz.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vns.zhongyouzk.top

TS:   if (s === "") {}
来源：http://wgv.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://vqg.jlsjyb.cn

Go:   if s == "" {}
来源：http://qfq.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://dit.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lsp.ybcxt.top

[E21] 超长截断加省略号
来源：http://yxu.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://exu.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://erx.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ghr.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jeh.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mkz.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://evt.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bzw.fktsv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wht.daria6918.cn

[E22] 字节长度与字符长度
来源：http://stx.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wvv.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qah.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hgx.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vgd.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mdf.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vmp.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://aez.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ckg.snrcjt.cn

================================================================================
来源：http://jsl.haohaochexian.top

F. 文件与目录
来源：http://vao.ctjpmb.com

================================================================================
来源：http://xzh.gzhubu.top

[F01] 读取整个文件
来源：http://xzj.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fgn.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://gwp.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zxc.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hdl.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tph.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ouk.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://yjb.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://whr.gogol.net.cn

[F02] 逐行读取文件
来源：http://osk.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://auo.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jpk.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://naz.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sgx.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yeb.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gpt.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jub.yj20258.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tam.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://mkx.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bjy.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://whh.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fls.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://thi.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lie.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ptj.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://cqd.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eua.jlsjyb.cn

[F04] 追加写入文件
来源：http://hue.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://csj.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jrj.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwq.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uqa.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wpl.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ijn.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cdk.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ebl.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://vrt.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iqx.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://ghr.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://rcg.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://rkt.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sxf.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nwi.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://ase.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://ofc.cqqwz.cn

[F06] 删除文件
来源：http://avk.daria6918.cn

Py:   os.remove("a.txt")
来源：http://knq.xuanzx.com

PHP:  unlink("a.txt");
来源：http://xrx.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://fwc.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vru.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lni.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://uen.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://rka.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://uyz.iojbl.cn

[F07] 创建目录（含多级）
来源：http://oqj.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmq.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hzt.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uzh.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nud.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ans.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ymg.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gaz.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fqo.xinyue.icu

[F08] 遍历目录
来源：http://ecy.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://abo.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ssw.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://wbp.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://qfb.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jbw.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ify.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://nii.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://nzd.cheryme.top

[F09] 获取文件大小
来源：http://pzz.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://gfp.meibo888.top

PHP:  filesize("a.txt");
来源：http://ekz.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://haf.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://cxp.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fvs.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://llz.yongpay.top

Ruby: File.size("a.txt")
来源：http://ema.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://jyg.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://tkw.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://juj.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cuq.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ijw.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://fud.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iwi.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://skh.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://div.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bpc.jlsjyb.cn

[F11] 复制与移动文件
来源：http://mti.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iwz.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mcf.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygq.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cef.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://upe.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://smh.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kif.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://snw.xziqi.cn

[F12] CSV 读写
来源：http://xky.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cym.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ksc.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gkm.bbcook.cn

TS:   // 同上
来源：http://nil.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ewb.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vft.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tja.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uzz.jyoumei.cn

================================================================================
来源：http://qju.quarkkingdee.top

G. 面向对象
来源：http://xno.daria6918.cn

================================================================================
来源：http://rwm.hcnkem.com

[G01] 定义类
来源：http://ydo.epnwcf.com

Py:   class User: pass
来源：http://vwm.zdbjq.cn

PHP:  class User {}
来源：http://gjd.sjlbkw.cn

JS:   class User {}
来源：http://kkx.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://bpf.ybcxt.top

Java: class User {}
来源：http://kua.fzhhl.top

Go:   type User struct { Name string }
来源：http://foa.ybcxt.top

Ruby: class User; end
来源：http://mtt.hnxiangtu.top

C#:   class User {}
来源：http://iuo.hcnkem.com

[G02] 构造函数
来源：http://yzs.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://ruv.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://bca.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://zzi.yongpay.top

TS:   constructor(public name: string) {}
来源：http://jas.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://qqx.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://abm.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://smg.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://xhr.ehwqpu.com

[G03] 实例属性
来源：http://rel.ctjpmb.com

Py:   self.name = "x"
来源：http://mdz.sysykeji.top

PHP:  public string $name = "x";
来源：http://axy.zhoulong.xyz


<!-- 参考信息 -->