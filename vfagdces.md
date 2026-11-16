代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zef.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tch.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvj.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oxq.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nsn.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ghd.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nav.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cli.52xcode.cn

[E06] 替换子串
来源：http://sad.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qyt.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://jjx.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ctk.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://zyb.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgc.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vvp.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wbr.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://jrc.52xcode.cn

[E07] 按分隔符拆分
来源：http://jsq.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://duq.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nzs.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://apj.ybcxt.top

TS:   s.split(",")
来源：http://yij.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://acf.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cug.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://xds.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvi.ybcxt.top

[E08] 数组按分隔符合并
来源：http://zhs.ivvv.top

Py:   ",".join(items)
来源：http://wzj.nwbrower.top

PHP:  implode(",", $items);
来源：http://zcy.dianchejie.cn

JS:   items.join(",")
来源：http://qdb.ivvv.top

TS:   items.join(",")
来源：http://bye.tianlin.xyz

Java: String.join(",", items)
来源：http://xie.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://xeg.jlsjyb.cn

Ruby: items.join(",")
来源：http://dbf.sysykeji.top

C#:   string.Join(",", items)
来源：http://vvs.fzhhl.top

[E09] 去除所有空白字符
来源：http://fxw.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ypd.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ads.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://wkj.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://mds.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://ypo.jiagoushi.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mkq.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://cbn.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cau.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://ojr.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bwx.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lsi.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://ovd.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://gyc.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://qcn.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aoq.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pbr.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qum.haohaochexian.top

[E11] 反转字符串
来源：http://erk.fengsongda.top

Py:   s[::-1]
来源：http://nbw.hnqzz.top

PHP:  strrev($s);
来源：http://ote.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://xed.yj202588.top

TS:   [...s].reverse().join("")
来源：http://xsh.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ras.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oki.xziqi.cn

Ruby: s.reverse
来源：http://oso.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://tua.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://oou.fzhhl.top

Py:   s.count("a")
来源：http://shh.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://mdl.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://mtp.hnqzz.top

TS:   s.split("a").length - 1
来源：http://esl.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://abb.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://ekh.chenjidiqi.icu

Ruby: s.count("a")
来源：http://nqr.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://qei.andypj.xyz

[E13] 逐字符遍历
来源：http://odz.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://sxj.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uyi.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lfv.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zhd.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xrp.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xua.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://kls.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qmr.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://xew.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fzk.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://nel.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hvh.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nfh.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bzq.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vdz.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ran.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vht.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://siu.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zfd.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pbu.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qrw.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pga.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ucl.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wac.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wzj.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nji.vqdsnc.cn

[E16] 数字千分位
来源：http://kte.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://nxl.xinyue.icu

PHP:  number_format(1234567);
来源：http://aws.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gec.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ihl.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zbx.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gax.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qkl.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://cge.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://ccb.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bms.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vir.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gvn.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bxv.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://swp.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gkm.sjlbkw.cn

Ruby: s.capitalize
来源：http://pxo.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hha.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://ayo.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dgn.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mvr.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dhn.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tlo.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kqz.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rmg.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mpj.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ltv.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://hmy.hysaishi.cn

Py:   s.splitlines()
来源：http://may.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dgf.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://roi.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://ngu.daxiang520.top

Java: s.lines().toList()
来源：http://vef.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://xev.jinyuanbaomall.cn

Ruby: s.lines
来源：http://net.9152youxi.cn

C#:   s.Split('\n')
来源：http://qdt.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://lkf.birdmap.top

Py:   if not s:
来源：http://bgc.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://daf.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rad.tanke756.top

TS:   if (s === "") {}
来源：http://vzg.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://vmb.xziqi.cn

Go:   if s == "" {}
来源：http://hnd.jlsjyb.cn

Ruby: if s.empty?
来源：http://ccc.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://skv.yonumen.top

[E21] 超长截断加省略号
来源：http://rff.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eos.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rmx.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cus.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dce.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lnc.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://zix.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://byh.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bfr.yj20258.top

[E22] 字节长度与字符长度
来源：http://nwy.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iaq.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://atq.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zar.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mho.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dbn.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wzj.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://mpz.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vov.gaohongyu789.top

================================================================================
来源：http://mcf.shanyushiyangkeji.top

F. 文件与目录
来源：http://nxm.hnxiangtu.top

================================================================================
来源：http://ptt.yuanzhike.top

[F01] 读取整个文件
来源：http://nqw.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dfv.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://kkr.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gam.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dqp.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qmz.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vsr.fzhhl.top

Ruby: File.read("a.txt")
来源：http://xqp.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://qrm.zdqjudy.top

[F02] 逐行读取文件
来源：http://uek.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pvg.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tft.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cug.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xjt.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tyn.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jnq.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ywg.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://waa.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://gdl.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://whg.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bun.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mdq.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwk.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rha.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://njh.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://vit.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ook.shzxlz.cn

[F04] 追加写入文件
来源：http://vvh.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pzd.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://juj.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyz.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rnz.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qnx.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jpf.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dli.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hwd.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://acd.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wtj.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://vvo.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://mus.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://vhn.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ryt.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qfd.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://eny.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://orm.yongpay.top

[F06] 删除文件
来源：http://mza.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://efk.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://fgp.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://bec.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://cid.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nik.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://iam.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://oak.ivvv.top

C#:   File.Delete("a.txt");
来源：http://pry.cashguo.top

[F07] 创建目录（含多级）
来源：http://kuc.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pbp.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sxx.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgl.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://juc.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vgp.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://deo.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zep.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xsh.jinghuilouyu.cn

[F08] 遍历目录
来源：http://ypm.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iaq.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xnu.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://vfl.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://wnt.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zfd.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://thb.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://vvh.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://zws.guowangkeji.top

[F09] 获取文件大小
来源：http://xqc.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://xze.uphjek.com

PHP:  filesize("a.txt");
来源：http://hlk.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://lge.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://wjj.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://adw.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ycn.shuidangran.top

Ruby: File.size("a.txt")
来源：http://elo.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://yet.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://wcf.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ydc.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eff.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hpl.sysykeji.top

TS:   path.extname("a.txt")
来源：http://gmh.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fwv.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://exk.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eea.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hnk.hfpthk.cn

[F11] 复制与移动文件
来源：http://nfu.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjx.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fpo.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://phy.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwo.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qdq.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mad.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sgd.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://shi.yj20258.top

[F12] CSV 读写
来源：http://xpc.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tee.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xsz.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mwf.yj20258.top

TS:   // 同上
来源：http://cav.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vby.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qfi.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fhc.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://apa.fanxiaobao.xyz

================================================================================
来源：http://ahe.zdqjudy.top

G. 面向对象
来源：http://zko.ehwqpu.com

================================================================================
来源：http://omb.jqgufenzy.top

[G01] 定义类
来源：http://vol.meibo888.top

Py:   class User: pass
来源：http://xjo.hcnkem.com

PHP:  class User {}
来源：http://ydu.zycfv.cn

JS:   class User {}
来源：http://hqi.pycfn.com

TS:   class User { name: string = ""; }
来源：http://qox.vqdsnc.cn

Java: class User {}
来源：http://hqy.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://cad.aizwys.cn

Ruby: class User; end
来源：http://fyp.gogol.net.cn

C#:   class User {}
来源：http://okq.jiagoushi.top

[G02] 构造函数
来源：http://ffu.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://qjn.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://wjl.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://axg.cashguo.top

TS:   constructor(public name: string) {}
来源：http://qvw.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://ece.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dfh.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://zlp.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://krv.guowangkeji.top

[G03] 实例属性
来源：http://vmm.pengpengdd.cyou

Py:   self.name = "x"
来源：http://xiu.c1oappe.top

PHP:  public string $name = "x";
来源：http://ctl.yj20258888.top

JS:   this.name = "x";
来源：http://zyg.meibo888.top

TS:   name: string = "x";
来源：http://tky.cheryme.top

Java: private String name;
来源：http://rag.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aar.daria6918.cn


<!-- 参考信息 -->