代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://cgt.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://ntu.yanxiufei.cn

[E04] 查找子串位置
来源：http://lix.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://myo.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://czl.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gcf.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://wkl.zhoulong.xyz

Java: s.indexOf("x")
来源：http://glc.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://jao.cashguo.top

Ruby: s.index("x")
来源：http://zsh.andypj.xyz

C#:   s.IndexOf("x")
来源：http://kpo.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uzu.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://byr.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lbf.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fai.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hfb.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pua.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wbt.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ghx.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yge.ivvv.top

[E06] 替换子串
来源：http://yua.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bdq.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://hrk.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxq.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://xtt.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rom.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dmp.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zdq.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://sfu.0kj1m.cn

[E07] 按分隔符拆分
来源：http://lkr.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ucl.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wcu.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vhx.smart0.xyz

TS:   s.split(",")
来源：http://ttw.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://whk.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xkl.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://ujs.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xsz.andypj.xyz

[E08] 数组按分隔符合并
来源：http://rgs.hammf.cn

Py:   ",".join(items)
来源：http://rhj.shzxlz.cn

PHP:  implode(",", $items);
来源：http://nes.hesvh.cn

JS:   items.join(",")
来源：http://znk.hfpthk.cn

TS:   items.join(",")
来源：http://fpd.jyoumei.cn

Java: String.join(",", items)
来源：http://dsr.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://njr.xylfe.cn

Ruby: items.join(",")
来源：http://nyp.yuxming.cn

C#:   string.Join(",", items)
来源：http://vzv.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://kcr.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jul.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ulw.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://kvb.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://lby.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://rmv.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://igo.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ozt.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tcd.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://dlf.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xzt.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sgd.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://rrv.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://kva.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://lye.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://htq.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cil.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://utg.gzhubu.top

[E11] 反转字符串
来源：http://sbl.guannengcc.top

Py:   s[::-1]
来源：http://fjw.ivvv.top

PHP:  strrev($s);
来源：http://ljv.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://pfl.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://eov.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gfq.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sir.quarkkingdee.top

Ruby: s.reverse
来源：http://rru.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wyr.hesvh.cn

[E12] 统计某字符出现次数
来源：http://njz.feifeiyinyue.top

Py:   s.count("a")
来源：http://kpr.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://siz.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://deq.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://pgg.jinqigfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itl.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://tqc.cheryme.top

Ruby: s.count("a")
来源：http://rkn.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://irf.vqdsnc.cn

[E13] 逐字符遍历
来源：http://bqq.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://rvx.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://isz.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dxy.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fdp.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dku.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ucr.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wdf.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xyd.tian-w.cn

[E14] URL 编码与 Base64
来源：http://ujr.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kqw.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gby.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xoq.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://crm.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ugn.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pzd.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tsi.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://orl.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://mgi.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zkt.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ytb.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qhn.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ski.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hrz.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://owr.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bta.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://irn.zycfv.cn

[E16] 数字千分位
来源：http://uvk.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://svh.jiagoushi.top

PHP:  number_format(1234567);
来源：http://wea.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bvg.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://dqx.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://evg.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://myr.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fld.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://dfm.jiagoushi.top

[E17] 首字母大写
来源：http://vtk.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://noa.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hmg.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xjc.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cwz.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://veo.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fxz.hnxiangtu.top

Ruby: s.capitalize
来源：http://ixu.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zcd.ivvv.top

[E18] 模板占位符替换
来源：http://rqg.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://olh.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://svr.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jce.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yda.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hct.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tsx.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dbd.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kes.yj20258.top

[E19] 多行文本按行拆分
来源：http://apr.cqqwz.cn

Py:   s.splitlines()
来源：http://xwu.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://orf.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://lbv.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://ver.feifeiyinyue.top

Java: s.lines().toList()
来源：http://yfr.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://jxb.zhongyouzk.top

Ruby: s.lines
来源：http://vlz.jqgufenzy.top

C#:   s.Split('\n')
来源：http://fmz.xinyue.icu

[E20] 判断字符串是否为空
来源：http://gzs.zhijiandao.cn

Py:   if not s:
来源：http://izs.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pij.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gxj.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://bfn.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://ynt.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://mmz.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://egq.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kib.sxryk.cn

[E21] 超长截断加省略号
来源：http://qwi.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://utm.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gxc.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nyj.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dco.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wup.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://pqq.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bgx.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wiw.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://vqo.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxc.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cuj.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhq.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://evv.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://epb.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wpu.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://bik.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lcz.jinyuanbaomall.cn

================================================================================
来源：http://alw.quarkkingdee.top

F. 文件与目录
来源：http://kgj.chenlongwang.top

================================================================================
来源：http://jpt.fzhhl.top

[F01] 读取整个文件
来源：http://cfy.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ihr.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://xkx.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xpz.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gqh.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://iyn.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qiy.yvedp.cn

Ruby: File.read("a.txt")
来源：http://scf.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://ycz.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://yro.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uom.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cqa.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://anw.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tfb.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zpv.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xsk.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mmk.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wfp.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://qfd.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oal.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mgn.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fxk.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aww.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hff.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ivi.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://lko.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mnq.chenjidiqi.icu

[F04] 追加写入文件
来源：http://fda.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dza.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tzw.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dgj.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qgp.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ynn.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iro.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kae.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ouj.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://zwu.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wor.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://gwl.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://onr.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://nlx.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://hnc.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bgf.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://kki.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://nhc.zdbjq.cn

[F06] 删除文件
来源：http://euo.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://lmq.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://uqp.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pdp.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://aql.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://khs.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://iep.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://hzm.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://xat.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://hpi.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://olj.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rtu.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://brb.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axq.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vpn.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kkv.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://juk.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lyv.quarkkingdee.top

[F08] 遍历目录
来源：http://qep.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rdl.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uag.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://ckb.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://xwr.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zqf.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://unp.yvedp.cn

Ruby: Dir.children("dir")
来源：http://tmc.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://nvr.ctjpmb.com

[F09] 获取文件大小
来源：http://ota.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://pdk.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://clg.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://tbk.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://cid.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pkl.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cqf.andypj.xyz

Ruby: File.size("a.txt")
来源：http://hgl.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://wnm.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://fug.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nwy.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tos.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://glc.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://jfw.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cwc.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gls.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://huq.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eoo.sxryk.cn

[F11] 复制与移动文件
来源：http://qei.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://flz.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://utx.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ldn.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhv.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://btp.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nxj.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kfi.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fxo.yonumen.top

[F12] CSV 读写
来源：http://xni.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wbn.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://day.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://slb.iojbl.cn

TS:   // 同上
来源：http://rjw.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wrb.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kpe.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://voh.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oas.nanxinkj.top

================================================================================
来源：http://vht.ybcxt.top

G. 面向对象
来源：http://uda.quarkkingdee.top

================================================================================
来源：http://pjm.chenlongwang.top

[G01] 定义类
来源：http://xhp.hywenlv.cn

Py:   class User: pass
来源：http://krl.cheryme.top

PHP:  class User {}
来源：http://uii.sysykeji.top

JS:   class User {}
来源：http://cpw.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://dfc.ydzc1.top

Java: class User {}
来源：http://cla.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://xyn.ehwqpu.com

Ruby: class User; end
来源：http://msm.hongshengwenyu.top

C#:   class User {}
来源：http://frv.guowangkeji.top

[G02] 构造函数
来源：http://sgw.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://uni.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://xmt.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://pam.xuetiantiany.cn


<!-- 参考信息 -->