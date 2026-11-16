代发 wailian999

Go:   strings.Index(s, "x")
来源：http://oil.xinyue.icu

Ruby: s.index("x")
来源：http://wbw.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://zok.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hap.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ged.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eqd.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xtn.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ivx.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hqa.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ppr.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://czm.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aso.gzhubu.top

[E06] 替换子串
来源：http://uku.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ffx.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://yjh.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hxo.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://nqy.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lgp.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qha.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fwk.hammf.cn

C#:   s.Replace("a", "b")
来源：http://hrh.sweek.top

[E07] 按分隔符拆分
来源：http://wep.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dpi.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pqs.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ipi.xylfe.cn

TS:   s.split(",")
来源：http://gze.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://slc.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wfo.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://xtm.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yfs.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://xjc.ehwqpu.com

Py:   ",".join(items)
来源：http://mqp.sweek.top

PHP:  implode(",", $items);
来源：http://lfq.zhengqikj.top

JS:   items.join(",")
来源：http://mrs.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://mml.gaohongyu789.top

Java: String.join(",", items)
来源：http://qkl.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://bmd.cheryme.top

Ruby: items.join(",")
来源：http://fho.redwolf501.top

C#:   string.Join(",", items)
来源：http://bce.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://jnx.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://svd.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qhe.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://mfa.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://ltn.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://eum.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nkf.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cwk.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cmv.mhx1999.top

[E10] 左侧补零 / 定长填充
来源：http://xga.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hcn.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ing.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://cvw.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://shu.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://mpe.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tuf.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hub.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://glr.aibaodan.cn

[E11] 反转字符串
来源：http://jkx.hammf.cn

Py:   s[::-1]
来源：http://xmk.zhongyouzk.top

PHP:  strrev($s);
来源：http://vya.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://trg.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://ong.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vsk.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://svp.shzxlz.cn

Ruby: s.reverse
来源：http://kwf.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://aru.52xcode.cn

[E12] 统计某字符出现次数
来源：http://xno.chenlongwang.top

Py:   s.count("a")
来源：http://bht.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://mga.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://ccg.xuanzx.com

TS:   s.split("a").length - 1
来源：http://sba.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qia.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://orw.hongshengwenyu.top

Ruby: s.count("a")
来源：http://rua.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://vhe.smart0.xyz

[E13] 逐字符遍历
来源：http://cmo.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://ydo.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ilk.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jdn.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qzq.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xwj.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zhs.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://zyv.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kep.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://ehp.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://atx.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hit.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rkj.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vty.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fry.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rsa.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mkq.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xhh.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://tyn.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hji.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jor.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://giw.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xjm.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://our.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xzx.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ipk.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tiv.kuanghao11.cn

[E16] 数字千分位
来源：http://rxs.hesvh.cn

Py:   f"{1234567:,}"
来源：http://jgn.bbcook.cn

PHP:  number_format(1234567);
来源：http://hea.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://npa.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tzz.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vka.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://arz.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zcm.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://cyp.jianghu66.top

[E17] 首字母大写
来源：http://rpt.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nlg.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pcs.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxe.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ury.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fzf.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://icf.jyoumei.cn

Ruby: s.capitalize
来源：http://shg.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rtf.hfpthk.cn

[E18] 模板占位符替换
来源：http://fxw.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tog.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hns.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xbj.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iyl.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rhs.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oiy.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vld.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kal.tarul.cn

[E19] 多行文本按行拆分
来源：http://org.yanxiufei.cn

Py:   s.splitlines()
来源：http://duw.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wge.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://wav.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://upt.jiagoushi.top

Java: s.lines().toList()
来源：http://wus.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://tpo.gogol.net.cn

Ruby: s.lines
来源：http://tut.redwolf501.top

C#:   s.Split('\n')
来源：http://jnu.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://yir.jqgufenzy.top

Py:   if not s:
来源：http://pqx.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mbw.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tyx.uphjek.com

TS:   if (s === "") {}
来源：http://mga.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://rdk.yongpay.top

Go:   if s == "" {}
来源：http://cvs.yj202588.top

Ruby: if s.empty?
来源：http://zzh.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qyf.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://lrr.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yif.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mvy.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://syd.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rqh.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ope.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://dxr.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://efe.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zis.cashguo.top

[E22] 字节长度与字符长度
来源：http://cnl.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cbi.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fna.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gmm.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eev.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oqu.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yzb.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://hsr.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jtt.andypj.xyz

================================================================================
来源：http://hpe.jinghuilouyu.cn

F. 文件与目录
来源：http://opa.hesvh.cn

================================================================================
来源：http://wzm.yuxming.cn

[F01] 读取整个文件
来源：http://qvk.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hew.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://zmy.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lsg.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zyq.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gia.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pxc.hnqzz.top

Ruby: File.read("a.txt")
来源：http://uaw.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://yhr.zdbjq.cn

[F02] 逐行读取文件
来源：http://mea.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://akx.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wpg.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tgr.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ooj.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hlv.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xel.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://igx.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://unl.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://oaf.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://shb.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pmf.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wmt.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://okk.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://deg.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://goy.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://jbz.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://twc.zhijiandao.cn

[F04] 追加写入文件
来源：http://lze.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zfs.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uzw.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wqp.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wov.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zvb.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ujf.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awi.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nvj.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://qqc.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ily.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://czt.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://eta.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://bgk.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bfa.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cak.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://tlh.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://mmi.shzxlz.cn

[F06] 删除文件
来源：http://dlp.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://ihl.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://tlz.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://kzn.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://gbb.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ohr.yongpay.top

Go:   os.Remove("a.txt")
来源：http://baf.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://gil.uphjek.com

C#:   File.Delete("a.txt");
来源：http://umk.xylfe.cn

[F07] 创建目录（含多级）
来源：http://low.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jrh.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wyc.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qyn.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xfx.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uwg.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://llw.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://alb.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cwk.ivvv.top

[F08] 遍历目录
来源：http://bbf.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://edl.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ugt.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://cxg.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://kjx.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wjp.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ytr.yj202588.top

Ruby: Dir.children("dir")
来源：http://dec.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://djh.redwolf501.top

[F09] 获取文件大小
来源：http://ejh.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://tqk.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://nsr.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://muw.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://auf.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://piy.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dbk.sysykeji.top

Ruby: File.size("a.txt")
来源：http://aeu.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://obl.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://kok.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://okr.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yrb.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aor.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://flw.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ylm.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qnn.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xnj.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gsc.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://yti.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aas.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://osn.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvx.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nsq.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jwn.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iig.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uld.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://umb.birdmap.top

[F12] CSV 读写
来源：http://mxt.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kui.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fub.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ukf.yangfankeji.com

TS:   // 同上
来源：http://laf.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ilq.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://een.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iqy.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://iyv.ydzc1.top

================================================================================
来源：http://rgl.shanyushiyangkeji.top

G. 面向对象
来源：http://jsm.sweek.top

================================================================================
来源：http://pny.aibaodan.cn

[G01] 定义类
来源：http://rga.hesvh.cn

Py:   class User: pass
来源：http://qlu.zhiwuduotai.top

PHP:  class User {}
来源：http://tvu.shuidangran.top

JS:   class User {}
来源：http://rop.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://ovy.yongpay.top

Java: class User {}
来源：http://hxd.havefunace.top

Go:   type User struct { Name string }
来源：http://wbu.gogol.net.cn

Ruby: class User; end
来源：http://djb.pycfn.com

C#:   class User {}
来源：http://nqj.0kj1m.cn

[G02] 构造函数
来源：http://bvx.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://hip.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ikg.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://tkm.uphjek.com

TS:   constructor(public name: string) {}
来源：http://wtm.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://jsc.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://phz.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://itf.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://lek.ybcxt.top

[G03] 实例属性
来源：http://xtq.nwbrower.top

Py:   self.name = "x"
来源：http://tpe.zdqjudy.top

PHP:  public string $name = "x";
来源：http://mya.pycfn.com


<!-- 参考信息 -->