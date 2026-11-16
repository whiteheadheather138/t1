代发 wailian999

[E02] 重复字符串
来源：http://goq.yuxming.cn

Py:   "ab" * 3
来源：http://vgm.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://ujr.hnqzz.top

JS:   "ab".repeat(3)
来源：http://syi.fehbvm.com

TS:   "ab".repeat(3)
来源：http://avd.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://ool.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://qub.cashguo.top

Ruby: "ab" * 3
来源：http://bmf.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fup.meibo888.top

[E03] 截取子串
来源：http://ztr.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aky.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cnm.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rvx.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://wro.gzhubu.top

Java: s.substring(1, 4)
来源：http://lxh.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ube.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://xia.birdmap.top

C#:   s.Substring(1, 3)
来源：http://cht.zhengqikj.top

[E04] 查找子串位置
来源：http://edw.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://qkm.yuxming.cn

PHP:  strpos($s, "x");
来源：http://iev.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uhu.uphjek.com

TS:   s.indexOf("x")
来源：http://ihv.zhoulong.xyz

Java: s.indexOf("x")
来源：http://kpg.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://hri.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://fwc.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://jnh.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rgw.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rjp.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aet.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lns.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://qjo.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cmj.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://emh.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dlp.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wrz.zhengqikj.top

[E06] 替换子串
来源：http://xsd.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bds.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://qyx.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gqa.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://sek.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zal.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rgd.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cgo.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://nnc.316326.xyz

[E07] 按分隔符拆分
来源：http://tcl.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://znn.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ebc.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xda.wangshuangyany.cn

TS:   s.split(",")
来源：http://orh.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://hrt.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kns.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://hms.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gze.pycfn.com

[E08] 数组按分隔符合并
来源：http://pte.dianchejie.cn

Py:   ",".join(items)
来源：http://wrw.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://tfl.redwolf501.top

JS:   items.join(",")
来源：http://lga.yonumen.top

TS:   items.join(",")
来源：http://hda.fzhhl.top

Java: String.join(",", items)
来源：http://srj.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://sxm.feifeiyinyue.top

Ruby: items.join(",")
来源：http://ykr.bbcook.cn

C#:   string.Join(",", items)
来源：http://ish.meibo888.top

[E09] 去除所有空白字符
来源：http://osl.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rcr.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mdg.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://uqg.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://mql.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://run.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pfn.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wlu.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tea.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://zim.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nnl.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rpy.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://gre.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://vhq.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://lwn.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hjq.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ulg.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jqq.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://omk.zhixingplan.top

Py:   s[::-1]
来源：http://hxb.fktsv.cn

PHP:  strrev($s);
来源：http://uwa.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://hoq.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://sri.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://boe.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://djd.andypj.xyz

Ruby: s.reverse
来源：http://jit.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://oan.daria6918.cn

[E12] 统计某字符出现次数
来源：http://xvb.ybcxt.top

Py:   s.count("a")
来源：http://oya.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://lfu.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://ttc.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://qhh.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hjk.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://yfi.zhongyouzk.top

Ruby: s.count("a")
来源：http://cmy.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://rob.aizwys.cn

[E13] 逐字符遍历
来源：http://pdz.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://eaf.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pcg.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://brh.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qsm.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ecs.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rpk.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vjm.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://clp.tarul.cn

[E14] URL 编码与 Base64
来源：http://xob.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ybx.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mps.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://joi.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ikc.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fah.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nyl.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jvr.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://goo.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://gcd.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pji.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rgn.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mns.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rjm.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcn.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uip.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rol.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eks.birdmap.top

[E16] 数字千分位
来源：http://gyf.mhx1999.top

Py:   f"{1234567:,}"
来源：http://dqj.jyoumei.cn

PHP:  number_format(1234567);
来源：http://fpu.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tjp.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://yzy.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nsg.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tom.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gou.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://sfg.shanyushiyangtech.top

[E17] 首字母大写
来源：http://xsp.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://amz.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yfi.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cgw.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eil.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xuy.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rgc.jyoumei.cn

Ruby: s.capitalize
来源：http://xfk.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mne.hfpthk.cn

[E18] 模板占位符替换
来源：http://myk.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eon.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pmc.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ccc.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://elt.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zao.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://trl.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blw.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nqu.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://evc.fzhhl.top

Py:   s.splitlines()
来源：http://jvh.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zlw.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://mxx.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://vpj.hesvh.cn

Java: s.lines().toList()
来源：http://zbo.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://dlk.shuidangran.top

Ruby: s.lines
来源：http://pve.jinqigfzy.top

C#:   s.Split('\n')
来源：http://gbn.fengsongda.top

[E20] 判断字符串是否为空
来源：http://dar.yuxming.cn

Py:   if not s:
来源：http://hnm.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jau.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bhv.havefunace.top

TS:   if (s === "") {}
来源：http://uuk.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://jdz.dianchejie.cn

Go:   if s == "" {}
来源：http://jiu.birdmap.top

Ruby: if s.empty?
来源：http://lsy.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://koh.mhx1999.top

[E21] 超长截断加省略号
来源：http://ypg.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pbu.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vyd.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tnw.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aag.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://max.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://ggc.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nwz.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bhu.zycfv.cn

[E22] 字节长度与字符长度
来源：http://pde.sufxvd.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vuo.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hex.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ykp.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pco.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://quq.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jea.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://sfl.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fwi.fktsv.cn

================================================================================
来源：http://vil.wangshuangyany.cn

F. 文件与目录
来源：http://vvh.dianchejie.cn

================================================================================
来源：http://dfc.yonumen.top

[F01] 读取整个文件
来源：http://qzh.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oqz.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://hax.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hxk.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rgo.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qej.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ljc.fzhhl.top

Ruby: File.read("a.txt")
来源：http://crw.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://rle.yfazqb.com

[F02] 逐行读取文件
来源：http://vnl.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sbt.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://twt.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edt.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://axg.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cjh.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nso.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gbm.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qha.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://cve.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dwf.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pzn.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nzy.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfn.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bln.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sbw.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://ijy.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://flv.jiagoushi.top

[F04] 追加写入文件
来源：http://two.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nyg.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://awy.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfo.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azs.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ilb.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uhi.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sdn.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kte.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://mwe.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kys.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://ezt.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://vsu.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://rci.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eoe.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zbc.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://txr.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://rdi.iojbl.cn

[F06] 删除文件
来源：http://yhv.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://gws.sysykeji.top

PHP:  unlink("a.txt");
来源：http://qxl.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://meb.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cwp.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bsy.cheryme.top

Go:   os.Remove("a.txt")
来源：http://vdk.yonumen.top

Ruby: File.delete("a.txt")
来源：http://non.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://rkh.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://nrl.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rpi.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ujb.snrcjt.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldi.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmw.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nfg.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://svq.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lzj.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gaj.chenzaomai.com

[F08] 遍历目录
来源：http://fys.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://wug.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://old.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://akc.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://liv.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oec.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mas.pycfn.com

Ruby: Dir.children("dir")
来源：http://uqk.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://jfb.316326.xyz

[F09] 获取文件大小
来源：http://ewb.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://mqg.yueranfly.top

PHP:  filesize("a.txt");
来源：http://lse.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://lgg.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://hno.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://awh.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oqq.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://vma.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://gyr.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://rrc.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://udv.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjb.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qgo.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://wni.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xpn.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://thk.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fnn.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://itj.fehbvm.com

[F11] 复制与移动文件
来源：http://msd.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ubl.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lnf.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://npf.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://asf.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qop.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ixg.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ahg.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vmm.quarkkingdee.top

[F12] CSV 读写
来源：http://gbq.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lbg.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qhm.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://brs.jinyuanbaomall.cn

TS:   // 同上
来源：http://ucd.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ekg.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uak.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jwe.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ahx.yangfankeji.com


<!-- 参考信息 -->