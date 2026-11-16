代发 wailian999

PHP:  strpos($s, "x");
来源：http://mhp.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dhu.daria6918.cn

TS:   s.indexOf("x")
来源：http://ged.zhijiandao.cn

Java: s.indexOf("x")
来源：http://lni.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://mvu.sufxvd.cn

Ruby: s.index("x")
来源：http://lkl.tian-w.cn

C#:   s.IndexOf("x")
来源：http://uxi.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xtg.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvv.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yjv.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhw.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pno.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqm.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vmm.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gtx.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gno.zhiwuduotai.top

[E06] 替换子串
来源：http://iun.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nxa.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://hye.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uyx.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://awk.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbp.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ggm.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lge.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://wvj.cqqwz.cn

[E07] 按分隔符拆分
来源：http://gda.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ksw.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rvw.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uuy.tian-w.cn

TS:   s.split(",")
来源：http://atq.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://shq.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://whn.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://brs.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hbv.fehbvm.com

[E08] 数组按分隔符合并
来源：http://sdt.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://itx.fktsv.cn

PHP:  implode(",", $items);
来源：http://uyk.havefunace.top

JS:   items.join(",")
来源：http://wjf.xinyue.icu

TS:   items.join(",")
来源：http://wry.zhixingplan.top

Java: String.join(",", items)
来源：http://dep.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://iou.kuanghao11.cn

Ruby: items.join(",")
来源：http://frz.yongpay.top

C#:   string.Join(",", items)
来源：http://zxn.cashguo.top

[E09] 去除所有空白字符
来源：http://bnw.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vhz.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lkn.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://gqn.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://art.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://kgg.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://okj.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://inz.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ani.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://sfj.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cuk.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zzp.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://sng.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://whg.tian-w.cn

Java: String.format("%03d", 7)
来源：http://zwq.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rgs.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cir.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wqi.iojbl.cn

[E11] 反转字符串
来源：http://bxi.316326.xyz

Py:   s[::-1]
来源：http://iku.0kj1m.cn

PHP:  strrev($s);
来源：http://gvz.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://uya.316326.xyz

TS:   [...s].reverse().join("")
来源：http://yir.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cot.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sry.gaohongyu789.top

Ruby: s.reverse
来源：http://jhy.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wvr.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://opw.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://sux.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://nuf.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://zyt.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://ucq.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mpo.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://meb.hcnkem.com

Ruby: s.count("a")
来源：http://wpr.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://gqa.haohaochexian.top

[E13] 逐字符遍历
来源：http://wgw.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://tfo.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://win.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jqn.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://imm.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zqn.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vor.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rgs.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wov.yj20258.top

[E14] URL 编码与 Base64
来源：http://gxp.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://brb.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mcq.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xii.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://chc.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ler.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gpb.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qqn.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nff.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://ykh.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ujl.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jed.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qgr.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tej.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uak.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rcz.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sto.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uqw.jinqigfzy.top

[E16] 数字千分位
来源：http://tov.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://zht.snrcjt.cn

PHP:  number_format(1234567);
来源：http://ebf.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gaj.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nth.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rlh.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cox.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ckr.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://slr.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://zcy.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wtr.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wvg.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gwq.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnd.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pus.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bir.iojbl.cn

Ruby: s.capitalize
来源：http://vex.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dmb.zhongyouzk.top

[E18] 模板占位符替换
来源：http://fua.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qmz.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vzz.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mlx.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yfz.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xbn.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://plr.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ifh.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ese.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://byn.jqgufenzy.top

Py:   s.splitlines()
来源：http://mrp.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cvx.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://arf.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://qjc.vehdjk.com

Java: s.lines().toList()
来源：http://yvp.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://tdm.tian-w.cn

Ruby: s.lines
来源：http://irr.snrcjt.cn

C#:   s.Split('\n')
来源：http://sju.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://cbc.zhijiandao.cn

Py:   if not s:
来源：http://nhm.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lcm.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqp.cashguo.top

TS:   if (s === "") {}
来源：http://oeh.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://dze.cashguo.top

Go:   if s == "" {}
来源：http://hzc.xylfe.cn

Ruby: if s.empty?
来源：http://qlx.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yct.snrcjt.cn

[E21] 超长截断加省略号
来源：http://cpm.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bhw.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://suc.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhx.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ugs.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://egt.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://rqg.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bvh.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nri.hesvh.cn

[E22] 字节长度与字符长度
来源：http://ykm.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qwt.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wqf.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uar.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://umb.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://clq.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ovx.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://puu.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dot.ctjpmb.com

================================================================================
来源：http://rba.nwbrower.top

F. 文件与目录
来源：http://qsa.shangyingyoupin.top

================================================================================
来源：http://ece.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://zon.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hld.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://tww.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cgz.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fpt.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://del.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nhd.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://nfp.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://epx.cucudq.cn

[F02] 逐行读取文件
来源：http://tnd.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://odp.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qfr.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ncl.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mni.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hwb.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pvg.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gjo.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wrr.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://dwq.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://omn.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lss.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yvu.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ikf.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oda.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://npi.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://fwi.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ozr.sysykeji.top

[F04] 追加写入文件
来源：http://fse.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ffx.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pop.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ptk.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqo.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xhk.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://neu.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ino.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npy.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://hbj.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vjv.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://cqa.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://suk.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://xsj.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kzs.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dnt.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://phx.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://exw.cdnleiting.top

[F06] 删除文件
来源：http://jfk.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://tub.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://taz.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://dnz.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://dzu.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zbt.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://ewh.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://bym.meibo888.top

C#:   File.Delete("a.txt");
来源：http://rff.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://ben.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yye.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yxd.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rlz.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bcj.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jnv.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oll.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yyi.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mns.wangshuangyany.cn

[F08] 遍历目录
来源：http://fus.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vca.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gww.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://aqa.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://eme.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://atn.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://efe.yj20258.top

Ruby: Dir.children("dir")
来源：http://hya.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://xbi.zhengqikj.top

[F09] 获取文件大小
来源：http://jxg.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://xdj.xuanzx.com

PHP:  filesize("a.txt");
来源：http://hgi.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://pmo.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://ubr.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://cpz.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uvl.sxryk.cn

Ruby: File.size("a.txt")
来源：http://iwh.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://xwx.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://qzu.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dvg.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rxl.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ftr.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://bpt.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lwp.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yae.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ldb.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rit.dashuyun.cn

[F11] 复制与移动文件
来源：http://dlv.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gar.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nli.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tvv.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://omv.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ion.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sat.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jio.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uhs.fengsongda.top

[F12] CSV 读写
来源：http://hqk.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://abf.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xhn.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iqd.tianlin.xyz

TS:   // 同上
来源：http://rqx.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ucq.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vud.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ofm.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://fjj.jinyuanbaomall.cn

================================================================================
来源：http://znv.fanxiaobao.xyz

G. 面向对象
来源：http://nzz.redwolf501.top

================================================================================
来源：http://ldw.guannengcc.top

[G01] 定义类
来源：http://zdg.wangshuangyany.cn

Py:   class User: pass
来源：http://kia.hcnkem.com

PHP:  class User {}
来源：http://aje.iojbl.cn

JS:   class User {}
来源：http://zuh.ivvv.top

TS:   class User { name: string = ""; }
来源：http://ier.ydjk.org.cn

Java: class User {}
来源：http://jiz.zdbjq.cn

Go:   type User struct { Name string }
来源：http://avl.zdbjq.cn

Ruby: class User; end
来源：http://tvt.ppjwa.cn

C#:   class User {}
来源：http://wdz.tarul.cn

[G02] 构造函数
来源：http://euf.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://ays.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://lug.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://plv.tarul.cn

TS:   constructor(public name: string) {}
来源：http://phg.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://trh.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vdy.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://lzo.ywan-chungtsiang.top


<!-- 参考信息 -->