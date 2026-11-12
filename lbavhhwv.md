代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://eca.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://odt.wangdashe.top

JS:   arr.join(", ")
来源：http://rue.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://tfi.jianghu66.top

Java: String.join(", ", list)
来源：http://lln.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://wjn.yfazqb.com

Ruby: arr.join(", ")
来源：http://kmb.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://pnz.feifeiyinyue.top

================================================================================
来源：http://lym.9152youxi.cn

E. 字符串处理
来源：http://vtg.zhaomingkeji.xyz

================================================================================
来源：http://lqm.jqgufenzy.top

[E01] 拼接字符串
来源：http://njr.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pfk.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lyz.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajh.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgp.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://poh.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wfi.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gqy.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mkl.ehwqpu.com

[E02] 重复字符串
来源：http://pmq.havefunace.top

Py:   "ab" * 3
来源：http://eqr.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://usl.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://tpm.smart0.xyz

TS:   "ab".repeat(3)
来源：http://rkf.epnwcf.com

Java: "ab".repeat(3)
来源：http://crx.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://ssp.bjfxy.top

Ruby: "ab" * 3
来源：http://awm.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dmw.cdnleiting.top

[E03] 截取子串
来源：http://yqj.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mtn.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mdi.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yje.fengsongda.top

TS:   s.slice(1, 4)
来源：http://inm.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://esm.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wzg.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://adi.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://vhb.hywenlv.cn

[E04] 查找子串位置
来源：http://dmu.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://rbn.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://cen.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bso.zdqjudy.top

TS:   s.indexOf("x")
来源：http://egb.hcnkem.com

Java: s.indexOf("x")
来源：http://dzb.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://wks.cheryme.top

Ruby: s.index("x")
来源：http://dqz.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://yvx.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lft.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jjm.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jls.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lok.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wbc.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bbg.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lgk.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://haa.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fxh.vqdsnc.cn

[E06] 替换子串
来源：http://rzy.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fol.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://wul.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldc.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://mnc.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cdc.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lgh.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ipb.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://jag.redwolf501.top

[E07] 按分隔符拆分
来源：http://pbr.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yno.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ecq.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://byb.redwolf501.top

TS:   s.split(",")
来源：http://ibz.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://olq.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxt.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://dcq.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mqv.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://tvc.nanxinkj.top

Py:   ",".join(items)
来源：http://jvd.shzxlz.cn

PHP:  implode(",", $items);
来源：http://yyw.sufxvd.cn

JS:   items.join(",")
来源：http://zic.meibo888.top

TS:   items.join(",")
来源：http://kbt.yvedp.cn

Java: String.join(",", items)
来源：http://sih.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://evk.pycfn.com

Ruby: items.join(",")
来源：http://ikx.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://qgy.tarul.cn

[E09] 去除所有空白字符
来源：http://wlh.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hxt.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ean.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://kfz.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://fvm.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://sja.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nll.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://nuw.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rgr.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://smu.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://thw.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dge.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://dmn.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://nxx.uphjek.com

Java: String.format("%03d", 7)
来源：http://rwv.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qvq.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://agc.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://box.kuanghao11.cn

[E11] 反转字符串
来源：http://eep.gogol.net.cn

Py:   s[::-1]
来源：http://uji.pycfn.com

PHP:  strrev($s);
来源：http://hpf.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://yrk.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://pjc.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sab.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://izi.vehdjk.com

Ruby: s.reverse
来源：http://jvp.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://vln.316326.xyz

[E12] 统计某字符出现次数
来源：http://ujf.chenjidiqi.icu

Py:   s.count("a")
来源：http://cgk.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://rlb.xinyue.icu

JS:   s.split("a").length - 1
来源：http://axv.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://udx.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mct.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://jqh.ivvv.top

Ruby: s.count("a")
来源：http://qno.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://hds.daria6918.cn

[E13] 逐字符遍历
来源：http://cts.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://gmi.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qae.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://abt.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lcl.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qlr.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wcc.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hbu.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dmy.xziqi.cn

[E14] URL 编码与 Base64
来源：http://bwj.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://igc.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qnz.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mki.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://obq.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ekc.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fxy.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wuj.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ukg.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://qxe.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sfl.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tui.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jsn.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ogh.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dch.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lvb.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mgh.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ser.yuxming.cn

[E16] 数字千分位
来源：http://jfg.hammf.cn

Py:   f"{1234567:,}"
来源：http://acn.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://xrm.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vev.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://azo.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lke.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jro.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mfc.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://fui.bjfxy.top

[E17] 首字母大写
来源：http://wsx.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://frm.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gmt.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evg.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hao.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ccn.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zar.jyoumei.cn

Ruby: s.capitalize
来源：http://qoz.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ryx.fzhhl.top

[E18] 模板占位符替换
来源：http://acn.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rom.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hra.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bhc.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pra.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mzf.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vfv.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://paa.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sus.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://eyn.sjlbkw.cn

Py:   s.splitlines()
来源：http://axe.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hdk.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://lkw.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://hoz.sufxvd.cn

Java: s.lines().toList()
来源：http://zrk.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://whc.pengpengdd.cyou

Ruby: s.lines
来源：http://mdn.vqdsnc.cn

C#:   s.Split('\n')
来源：http://ofx.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://bel.zhijiandao.cn

Py:   if not s:
来源：http://owy.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cld.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bjf.zdbjq.cn

TS:   if (s === "") {}
来源：http://txc.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://fma.zhoulong.xyz

Go:   if s == "" {}
来源：http://krp.cucudq.cn

Ruby: if s.empty?
来源：http://cuk.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zwa.yueranfly.top

[E21] 超长截断加省略号
来源：http://hif.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qcx.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dbw.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmi.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qfy.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ojm.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://fph.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axo.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://itg.xinyue.icu

[E22] 字节长度与字符长度
来源：http://rdn.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jik.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://amp.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vlx.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ycj.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ojn.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eze.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://bfa.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qtt.yanxiufei.cn

================================================================================
来源：http://jqp.daria6918.cn

F. 文件与目录
来源：http://xrl.yueranfly.top

================================================================================
来源：http://nck.bjfxy.top

[F01] 读取整个文件
来源：http://omw.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jlq.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://uda.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jlu.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://emq.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wnq.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://btt.fengsongda.top

Ruby: File.read("a.txt")
来源：http://pdw.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://qlz.gogol.net.cn

[F02] 逐行读取文件
来源：http://kgd.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qou.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hrz.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lgt.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ltx.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hfn.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jvl.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rho.hywenlv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://req.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://mkn.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ftt.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xaz.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rmn.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bcn.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://phv.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uvc.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://weq.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cwd.fzhhl.top

[F04] 追加写入文件
来源：http://lkj.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://alk.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cwa.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nem.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vll.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zru.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wbk.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uij.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yru.sweek.top

[F05] 判断文件或目录是否存在
来源：http://pjo.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sto.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://nvk.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://hqy.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://nso.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://tzo.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zfr.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://mdj.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://vfr.hysaishi.cn

[F06] 删除文件
来源：http://ukm.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://mfu.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://iab.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://het.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://oqi.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://apl.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://tgs.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://omb.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://fps.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://jqj.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lfe.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rce.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qiq.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hsi.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nke.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://owh.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xkz.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xrm.iojbl.cn

[F08] 遍历目录
来源：http://krw.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mna.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kts.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://aeg.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://asu.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ecu.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dee.c1oappe.top

Ruby: Dir.children("dir")
来源：http://bwb.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://ezs.zhijiandao.cn

[F09] 获取文件大小
来源：http://ujz.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://xsg.tian-w.cn

PHP:  filesize("a.txt");
来源：http://djf.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://jxd.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://rkx.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://vcv.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dqc.tarul.cn

Ruby: File.size("a.txt")
来源：http://apv.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://jms.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://iks.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zpg.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ckz.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zxg.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://svs.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wba.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://myx.hywenlv.cn


<!-- 参考信息 -->