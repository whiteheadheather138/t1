代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jvl.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://obg.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iny.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://img.yvedp.cn

[E02] 重复字符串
来源：http://kzr.epnwcf.com

Py:   "ab" * 3
来源：http://btx.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://wtz.daxiang520.top

JS:   "ab".repeat(3)
来源：http://nfe.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://sqk.haohaochexian.top

Java: "ab".repeat(3)
来源：http://ogj.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://qji.guowangkeji.top

Ruby: "ab" * 3
来源：http://shf.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gpt.cucudq.cn

[E03] 截取子串
来源：http://pew.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rty.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fvt.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aei.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://iqk.xylfe.cn

Java: s.substring(1, 4)
来源：http://nne.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wjp.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mlq.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://weu.sjlbkw.cn

[E04] 查找子串位置
来源：http://pgd.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://rqs.tarul.cn

PHP:  strpos($s, "x");
来源：http://igf.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pfs.zycfv.cn

TS:   s.indexOf("x")
来源：http://uop.ctjpmb.com

Java: s.indexOf("x")
来源：http://pel.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://qux.zdbjq.cn

Ruby: s.index("x")
来源：http://pxm.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://xmg.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://cvf.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fjf.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yla.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gsc.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://myb.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjf.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qvx.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://olz.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cqe.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://oxz.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqo.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://lcp.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://asl.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://fxz.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yex.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rle.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umd.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://dve.ybcxt.top

[E07] 按分隔符拆分
来源：http://ejs.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qwd.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ebp.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wmn.daria6918.cn

TS:   s.split(",")
来源：http://mhp.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://set.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kme.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://rhi.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://azk.daria6918.cn

[E08] 数组按分隔符合并
来源：http://nlq.yvedp.cn

Py:   ",".join(items)
来源：http://frm.0kj1m.cn

PHP:  implode(",", $items);
来源：http://reb.zdbjq.cn

JS:   items.join(",")
来源：http://xdg.vehdjk.com

TS:   items.join(",")
来源：http://hkn.jqgufenzy.top

Java: String.join(",", items)
来源：http://usv.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://srb.dianchejie.cn

Ruby: items.join(",")
来源：http://xrk.yuanzhike.top

C#:   string.Join(",", items)
来源：http://ssk.chenlongwang.top

[E09] 去除所有空白字符
来源：http://yed.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://duz.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://new.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://fgr.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://goh.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://zwr.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wux.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://acb.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uyh.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://gdn.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mbx.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iqi.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://vic.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://kvm.ivvv.top

Java: String.format("%03d", 7)
来源：http://kow.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ekj.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bts.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pmp.sysykeji.top

[E11] 反转字符串
来源：http://vog.xziqi.cn

Py:   s[::-1]
来源：http://bpo.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://vys.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://uwf.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://axv.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://kzv.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jew.wangshuangyany.cn

Ruby: s.reverse
来源：http://htc.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://oda.epnwcf.com

[E12] 统计某字符出现次数
来源：http://dqa.sxryk.cn

Py:   s.count("a")
来源：http://iqy.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://ldl.iojbl.cn

JS:   s.split("a").length - 1
来源：http://uej.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://yqp.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kio.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://zgs.hongshengwenyu.top

Ruby: s.count("a")
来源：http://ior.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://fgw.cucudq.cn

[E13] 逐字符遍历
来源：http://wxe.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://ldm.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gbi.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://efj.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vrb.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yvc.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yap.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qor.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zfc.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://njg.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hem.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dlu.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://meq.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tgi.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mfv.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://egw.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://job.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ium.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://pvk.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://izv.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vio.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gid.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jnz.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nqd.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xzg.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zme.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btp.redwolf501.top

[E16] 数字千分位
来源：http://opa.aizwys.cn

Py:   f"{1234567:,}"
来源：http://xjb.daria6918.cn

PHP:  number_format(1234567);
来源：http://sjd.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bnp.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fhr.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bka.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://chh.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xwr.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://cwr.tianlin.xyz

[E17] 首字母大写
来源：http://bqd.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rqr.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ggh.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lnx.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zdi.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uzo.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pun.xinyue.icu

Ruby: s.capitalize
来源：http://dnz.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pwn.zycfv.cn

[E18] 模板占位符替换
来源：http://kex.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dan.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wnl.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sta.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cnf.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ipq.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://coa.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xrw.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dde.xinyue.icu

[E19] 多行文本按行拆分
来源：http://cdx.bbcook.cn

Py:   s.splitlines()
来源：http://lpw.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nar.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://zzo.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://fxa.jyoumei.cn

Java: s.lines().toList()
来源：http://hzu.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://kbg.cdnleiting.top

Ruby: s.lines
来源：http://mwc.jiagoushi.top

C#:   s.Split('\n')
来源：http://ttd.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://ygk.yueranfly.top

Py:   if not s:
来源：http://lki.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mrp.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hrj.sjlbkw.cn

TS:   if (s === "") {}
来源：http://xxa.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://szn.yj20258888.top

Go:   if s == "" {}
来源：http://xxm.tarul.cn

Ruby: if s.empty?
来源：http://eau.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ctu.yj202588.top

[E21] 超长截断加省略号
来源：http://cse.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pua.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://axj.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pyz.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmm.zhoulong.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kmy.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://ezn.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jyl.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lcx.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://njl.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://npn.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://opt.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxv.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fvi.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yuz.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cpu.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://gkq.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vuf.316326.xyz

================================================================================
来源：http://qus.ywan-chungtsiang.top

F. 文件与目录
来源：http://imi.gotoacloud.top

================================================================================
来源：http://yga.jqgfzy.top

[F01] 读取整个文件
来源：http://ing.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dom.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://yay.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://udu.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dsu.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://onn.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://exe.316326.xyz

Ruby: File.read("a.txt")
来源：http://rjv.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://fsn.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://ybr.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://czq.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://edm.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wht.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nud.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://udj.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://twc.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tra.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kdt.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://rkg.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blm.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nri.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bvr.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voq.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qxc.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmf.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://gxz.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tic.jqgufenzy.top

[F04] 追加写入文件
来源：http://jwn.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pso.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://asc.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvo.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwy.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://smc.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gsa.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wjp.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pvu.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://ctk.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vmf.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://ewj.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://ueh.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://iuz.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dvu.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iyo.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://hwk.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://lyd.cqqwz.cn

[F06] 删除文件
来源：http://tjt.cashguo.top

Py:   os.remove("a.txt")
来源：http://zaj.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://pap.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pgb.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://oac.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://usr.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://shy.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://dnk.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://chv.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://fwq.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://enc.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qon.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pjo.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rjd.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vns.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wze.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uxi.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xoq.fktsv.cn

[F08] 遍历目录
来源：http://qps.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ukp.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyc.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://yog.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://kvl.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ceh.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uxe.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://mqn.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://wnq.wangshuangyany.cn

[F09] 获取文件大小
来源：http://vnc.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://rrx.xuanzx.com

PHP:  filesize("a.txt");
来源：http://kau.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://oer.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://zhk.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://alf.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://man.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://drq.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://gma.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://hdt.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://obu.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjc.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oww.hammf.cn

TS:   path.extname("a.txt")
来源：http://hpa.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ycv.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mgq.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hzd.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vmg.ydjk.org.cn

[F11] 复制与移动文件
来源：http://tir.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dis.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ahg.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pjq.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygb.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kfk.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ivf.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uoc.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rtk.cashguo.top

[F12] CSV 读写
来源：http://ffi.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://itw.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://owl.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xfo.wangdashe.top

TS:   // 同上
来源：http://jbn.yuxming.cn


<!-- 参考信息 -->