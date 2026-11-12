代发 wailian999

[E02] 重复字符串
来源：http://tje.quarkkingdee.top

Py:   "ab" * 3
来源：http://qzx.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://yym.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://nbt.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://ojz.cqqwz.cn

Java: "ab".repeat(3)
来源：http://fip.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://cam.mhx1999.top

Ruby: "ab" * 3
来源：http://jql.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://faa.cashguo.top

[E03] 截取子串
来源：http://mqr.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://quz.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hfl.ybcxt.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dyr.andypj.xyz

TS:   s.slice(1, 4)
来源：http://ajn.andypj.xyz

Java: s.substring(1, 4)
来源：http://dzh.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fmu.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://dfc.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://kli.pengpengdd.cyou

[E04] 查找子串位置
来源：http://mwr.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://twd.xinyue.icu

PHP:  strpos($s, "x");
来源：http://nhv.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bhl.fktsv.cn

TS:   s.indexOf("x")
来源：http://ife.kuanghao11.cn

Java: s.indexOf("x")
来源：http://ugs.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://nye.hongshengwenyu.top

Ruby: s.index("x")
来源：http://zpq.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://nuf.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://reu.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rap.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hkc.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jix.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://suv.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egr.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pxf.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zvl.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jtl.yanxiufei.cn

[E06] 替换子串
来源：http://yiv.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://unv.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://ppg.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oxe.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://iih.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tls.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uzw.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pif.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://pfi.dianchejie.cn

[E07] 按分隔符拆分
来源：http://lyp.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bcl.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://exv.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pvw.jyoumei.cn

TS:   s.split(",")
来源：http://lmp.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://erm.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uds.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://ltm.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gkj.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://syb.ctjpmb.com

Py:   ",".join(items)
来源：http://sgj.fzhhl.top

PHP:  implode(",", $items);
来源：http://svy.jinqigfzy.top

JS:   items.join(",")
来源：http://ibf.pengpengdd.cyou

TS:   items.join(",")
来源：http://kca.ivvv.top

Java: String.join(",", items)
来源：http://kmt.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://nxf.hammf.cn

Ruby: items.join(",")
来源：http://gsm.fktsv.cn

C#:   string.Join(",", items)
来源：http://qtn.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://spp.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ypo.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rhh.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://izr.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://rky.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://gtg.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://crv.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://dmm.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fgr.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://dtw.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dpm.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mhh.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://zba.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://qlc.vehdjk.com

Java: String.format("%03d", 7)
来源：http://bmf.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://and.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zns.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hgw.yangfankeji.com

[E11] 反转字符串
来源：http://mls.zhijiandao.cn

Py:   s[::-1]
来源：http://fvl.yuxming.cn

PHP:  strrev($s);
来源：http://pkg.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://esr.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://von.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jdg.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sml.dianchejie.cn

Ruby: s.reverse
来源：http://ahv.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://tjx.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://feh.gogol.net.cn

Py:   s.count("a")
来源：http://euo.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://lxt.uphjek.com

JS:   s.split("a").length - 1
来源：http://tyy.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://tja.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cii.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://krd.bjfxy.top

Ruby: s.count("a")
来源：http://ckv.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://qtt.shuidangran.top

[E13] 逐字符遍历
来源：http://jut.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://ukg.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdm.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rzk.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qqp.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hok.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://msb.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hcr.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qne.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://vhu.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jiy.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gnv.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yuo.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pwv.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zdf.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xev.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dvn.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lpv.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://xtt.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tvi.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ooe.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wxe.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ufw.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://azt.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dan.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pqg.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bvy.zhixingplan.top

[E16] 数字千分位
来源：http://vtb.uphjek.com

Py:   f"{1234567:,}"
来源：http://isl.ppjwa.cn

PHP:  number_format(1234567);
来源：http://czs.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cte.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tib.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dfr.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mch.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sbr.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://dau.kuanghao11.cn

[E17] 首字母大写
来源：http://ewd.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uey.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://azj.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wqj.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://izj.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dpq.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ucd.cqqwz.cn

Ruby: s.capitalize
来源：http://ier.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://obk.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://kde.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hlg.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bko.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pto.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ofv.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://twm.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ljl.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ylv.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jpm.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://lia.yuxming.cn

Py:   s.splitlines()
来源：http://ncq.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ymj.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://frk.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://bim.pycfn.com

Java: s.lines().toList()
来源：http://tdd.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://ztu.tian-w.cn

Ruby: s.lines
来源：http://hpk.chenlongwang.top

C#:   s.Split('\n')
来源：http://qsn.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://wci.shanyushiyangtech.top

Py:   if not s:
来源：http://ouz.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://adt.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gbo.zhoulong.xyz

TS:   if (s === "") {}
来源：http://vnu.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://iet.birdmap.top

Go:   if s == "" {}
来源：http://qxj.vehdjk.com

Ruby: if s.empty?
来源：http://acn.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bpj.yj202588.top

[E21] 超长截断加省略号
来源：http://tst.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gwo.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jye.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bei.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://avl.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ymb.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://ows.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ylq.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://reh.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://gaw.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jdm.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ffg.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ylz.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yrb.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lfv.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xwv.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://jfl.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ldi.ydjk.org.cn

================================================================================
来源：http://dia.zhongyouzk.top

F. 文件与目录
来源：http://lcv.gotoacloud.top

================================================================================
来源：http://gkb.zhengqikj.top

[F01] 读取整个文件
来源：http://fmz.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ztb.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://drf.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tgs.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fjw.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://brw.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rxn.ybcxt.top

Ruby: File.read("a.txt")
来源：http://aqs.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ivj.kuanghao11.cn

[F02] 逐行读取文件
来源：http://nae.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hdk.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uas.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugw.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fer.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qbv.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oip.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ddf.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jqh.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://lbq.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tty.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://upm.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kul.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ial.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uir.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://njc.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://ewf.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yrr.ivvv.top

[F04] 追加写入文件
来源：http://zjo.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lwd.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jwf.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://itr.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pay.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aac.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qsp.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hfp.snrcjt.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ncr.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://cpq.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ggz.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://til.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://lqo.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://irt.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zzb.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hec.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://ush.sweek.top

C#:   File.Exists("a.txt")
来源：http://svd.aibaodan.cn

[F06] 删除文件
来源：http://frs.cheryme.top

Py:   os.remove("a.txt")
来源：http://nnz.hnqzz.top

PHP:  unlink("a.txt");
来源：http://cgw.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iyn.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://efq.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qzi.316326.xyz

Go:   os.Remove("a.txt")
来源：http://val.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://buy.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://ydu.guannengcc.top

[F07] 创建目录（含多级）
来源：http://oun.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://spk.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://scf.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://udl.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://arb.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pvc.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ckk.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vmm.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oei.nanxuanxn.top

[F08] 遍历目录
来源：http://fqd.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zrh.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iox.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://cxb.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://jvp.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qav.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yua.xylfe.cn

Ruby: Dir.children("dir")
来源：http://gua.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://ojm.ctjpmb.com

[F09] 获取文件大小
来源：http://qpc.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://lgr.bjfxy.top

PHP:  filesize("a.txt");
来源：http://bnb.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://zzy.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://ogv.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://wgj.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kle.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://toh.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://cpk.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://lmo.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zdr.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://esx.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uvu.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://vho.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ehx.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uwd.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vch.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eqc.cheryme.top

[F11] 复制与移动文件
来源：http://jyy.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mny.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xot.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nxo.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jmr.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ith.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jkp.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mjg.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://paf.gotoacloud.top

[F12] CSV 读写
来源：http://rbt.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ebe.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mfc.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jpa.chenlongwang.top

TS:   // 同上
来源：http://sec.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zud.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wcd.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rzt.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oyc.shanyushiyangtech.top


<!-- 参考信息 -->