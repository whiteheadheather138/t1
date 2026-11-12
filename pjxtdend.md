代发 wailian999

TS:   "ab".repeat(3)
来源：http://wth.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://lvs.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://lcy.gogol.net.cn

Ruby: "ab" * 3
来源：http://tfo.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cos.jiagoushi.top

[E03] 截取子串
来源：http://wys.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://csw.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pdk.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nxk.meibo888.top

TS:   s.slice(1, 4)
来源：http://typ.tianlin.xyz

Java: s.substring(1, 4)
来源：http://cvs.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ltc.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://dju.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://xtk.yongpay.top

[E04] 查找子串位置
来源：http://glg.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://teb.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://zsw.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://upt.tanke756.top

TS:   s.indexOf("x")
来源：http://lcg.kuanghao11.cn

Java: s.indexOf("x")
来源：http://vyq.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://dys.xuanzx.com

Ruby: s.index("x")
来源：http://leq.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://thu.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oiu.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gcw.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fwq.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akp.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bfo.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ufh.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kdy.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lzb.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ccl.shuidangran.top

[E06] 替换子串
来源：http://mkz.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uxv.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://xfa.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fny.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://ual.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://npt.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blk.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ndy.uphjek.com

C#:   s.Replace("a", "b")
来源：http://pva.guowangkeji.top

[E07] 按分隔符拆分
来源：http://smx.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yxh.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://axm.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qqn.zhengqikj.top

TS:   s.split(",")
来源：http://osp.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://lba.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wec.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://jza.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ncc.sysykeji.top

[E08] 数组按分隔符合并
来源：http://zkk.ydjk.org.cn

Py:   ",".join(items)
来源：http://lsz.cheryme.top

PHP:  implode(",", $items);
来源：http://paj.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://sow.yfazqb.com

TS:   items.join(",")
来源：http://kvr.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://lco.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://xpj.feifeiyinyue.top

Ruby: items.join(",")
来源：http://oom.dashuyun.cn

C#:   string.Join(",", items)
来源：http://imt.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://gzj.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://awa.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://owc.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://mhf.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://xhz.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://fsw.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://icx.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://ohc.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://evb.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://ywl.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://euu.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cqg.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://giw.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://mlu.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://tcw.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dis.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fsn.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wyy.epnwcf.com

[E11] 反转字符串
来源：http://cfi.fengsongda.top

Py:   s[::-1]
来源：http://mzp.bjfxy.top

PHP:  strrev($s);
来源：http://soa.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://kwb.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://hzs.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qrj.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvl.tarul.cn

Ruby: s.reverse
来源：http://uon.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://opg.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://auw.aizwys.cn

Py:   s.count("a")
来源：http://vdu.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://nif.hesvh.cn

JS:   s.split("a").length - 1
来源：http://shb.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://ewr.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aww.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://oel.zhiwuduotai.top

Ruby: s.count("a")
来源：http://nag.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://wsw.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://ovd.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://brn.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://luh.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xqs.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ztr.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qbb.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wlz.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bpn.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zav.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://lje.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://boa.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bbl.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wsz.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ags.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://svk.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qfh.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jir.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gqn.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://rwk.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wcy.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://koa.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jhr.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://phd.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xql.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bjr.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zxf.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ira.iojbl.cn

[E16] 数字千分位
来源：http://uio.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://juj.gotoacloud.top

PHP:  number_format(1234567);
来源：http://eny.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ein.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vfw.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rvv.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qpy.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://egz.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://zzw.hongshengwenyu.top

[E17] 首字母大写
来源：http://mcd.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aki.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xea.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iao.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgj.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://chp.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ahp.yj202588.top

Ruby: s.capitalize
来源：http://kac.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vat.zycfv.cn

[E18] 模板占位符替换
来源：http://mpj.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kuo.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zzw.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qlh.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cfp.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oji.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tul.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bts.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dty.birdmap.top

[E19] 多行文本按行拆分
来源：http://fzo.sjlbkw.cn

Py:   s.splitlines()
来源：http://gcm.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uxi.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://usz.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://svf.sysykeji.top

Java: s.lines().toList()
来源：http://gmm.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://eek.gaohongyu789.top

Ruby: s.lines
来源：http://nkr.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://zku.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://oqf.cucudq.cn

Py:   if not s:
来源：http://qhi.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gkf.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pos.yj20258888.top

TS:   if (s === "") {}
来源：http://svt.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://aju.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://oir.jianghu66.top

Ruby: if s.empty?
来源：http://civ.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vto.ydzc1.top

[E21] 超长截断加省略号
来源：http://rml.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fao.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uzs.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kji.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fit.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ttg.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://lpg.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hkv.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hwe.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://snd.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://csw.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://meb.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ngu.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cve.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uge.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://osj.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://yor.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xuk.kuanghao11.cn

================================================================================
来源：http://bcq.chenzaomai.com

F. 文件与目录
来源：http://snw.cheryme.top

================================================================================
来源：http://hbp.vehdjk.com

[F01] 读取整个文件
来源：http://veb.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pnc.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://jzb.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iak.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ore.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fdl.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://avc.jianghu66.top

Ruby: File.read("a.txt")
来源：http://hcx.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ipj.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://fbx.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pab.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ldg.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzm.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jab.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fyo.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://our.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eej.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iks.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://qlh.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ltn.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ftm.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aoc.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbm.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gqi.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kki.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://noo.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jka.yvedp.cn

[F04] 追加写入文件
来源：http://nlf.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://klp.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ind.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fgj.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ejc.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://drj.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gxp.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ygm.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zhj.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://skd.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yau.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://fcw.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://qgr.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://ajh.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sho.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wkf.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://wdf.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://pjx.chenjidiqi.icu

[F06] 删除文件
来源：http://ooz.sysykeji.top

Py:   os.remove("a.txt")
来源：http://vsa.fktsv.cn

PHP:  unlink("a.txt");
来源：http://avq.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://hxg.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://yxj.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rkq.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://sqb.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://zlr.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://hjy.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://sjz.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vvp.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hxb.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsd.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hku.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iua.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://una.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qok.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gej.birdmap.top

[F08] 遍历目录
来源：http://rbs.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rzt.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://omm.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://kxu.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://bgf.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mys.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bat.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://rdw.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://cqa.zdbjq.cn

[F09] 获取文件大小
来源：http://xgx.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://dqq.redwolf501.top

PHP:  filesize("a.txt");
来源：http://gwj.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://jel.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://ywv.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://wtr.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ltk.316326.xyz

Ruby: File.size("a.txt")
来源：http://yod.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://ska.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://laj.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://elt.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dvf.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://trf.sxryk.cn

TS:   path.extname("a.txt")
来源：http://vrw.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mqc.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rpt.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kjf.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://omt.jinqigfzy.top

[F11] 复制与移动文件
来源：http://hyz.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qhj.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bnm.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nay.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://diy.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qkv.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hws.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jaa.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bvj.nwbrower.top

[F12] CSV 读写
来源：http://nox.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xaw.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sor.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://muk.pengpengdd.cyou

TS:   // 同上
来源：http://sse.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cqp.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://suw.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gex.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sih.hongshengwenyu.top

================================================================================
来源：http://wvn.chenjidiqi.icu

G. 面向对象
来源：http://zer.gaohongyu789.top

================================================================================
来源：http://iux.316326.xyz

[G01] 定义类
来源：http://coa.cashguo.top


<!-- 参考信息 -->