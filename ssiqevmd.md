代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yxp.ybcxt.top

[E03] 截取子串
来源：http://yvw.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gie.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ziy.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cjy.ivvv.top

TS:   s.slice(1, 4)
来源：http://jfo.ppjwa.cn

Java: s.substring(1, 4)
来源：http://rtv.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ajq.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://wji.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://mkb.hammf.cn

[E04] 查找子串位置
来源：http://lvy.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://xgb.yj202588.top

PHP:  strpos($s, "x");
来源：http://tty.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kqf.yueranfly.top

TS:   s.indexOf("x")
来源：http://oor.gzhubu.top

Java: s.indexOf("x")
来源：http://rsp.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://sje.dianchejie.cn

Ruby: s.index("x")
来源：http://njy.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://fhd.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cle.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://btr.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ohu.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tmz.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://abh.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hgu.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://szk.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ogo.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yji.sysykeji.top

[E06] 替换子串
来源：http://bpy.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vzu.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://obl.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcs.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://muz.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rsf.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://knb.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dig.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://cbb.bbcook.cn

[E07] 按分隔符拆分
来源：http://kdy.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zaj.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mii.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eoa.vqdsnc.cn

TS:   s.split(",")
来源：http://hsb.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://roc.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vej.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://dlz.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dun.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://koi.daria6918.cn

Py:   ",".join(items)
来源：http://kjd.epnwcf.com

PHP:  implode(",", $items);
来源：http://kkc.tarul.cn

JS:   items.join(",")
来源：http://otn.zhengqikj.top

TS:   items.join(",")
来源：http://kty.zhijiandao.cn

Java: String.join(",", items)
来源：http://vii.hammf.cn

Go:   strings.Join(items, ",")
来源：http://zqc.iojbl.cn

Ruby: items.join(",")
来源：http://aeo.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://izd.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://vgg.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pgl.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nhl.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://ime.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://awp.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://vzt.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://pup.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://lma.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kml.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://zxx.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ayd.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jkj.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://moo.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://rcx.yangfankeji.com

Java: String.format("%03d", 7)
来源：http://mbr.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tym.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nuq.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cnn.tianlin.xyz

[E11] 反转字符串
来源：http://fug.shzxlz.cn

Py:   s[::-1]
来源：http://ita.jiagoushi.top

PHP:  strrev($s);
来源：http://pae.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://bhn.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://xbz.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hrj.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fbj.ydjk.org.cn

Ruby: s.reverse
来源：http://mqe.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tky.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://yrk.jlsjyb.cn

Py:   s.count("a")
来源：http://wjo.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://jqn.andypj.xyz

JS:   s.split("a").length - 1
来源：http://qfo.tian-w.cn

TS:   s.split("a").length - 1
来源：http://dqq.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://efb.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://uqx.jqgufenzy.top

Ruby: s.count("a")
来源：http://aod.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://shb.zhijiandao.cn

[E13] 逐字符遍历
来源：http://dvr.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://qdx.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nah.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kko.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ash.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://btf.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jgx.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://afc.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uzv.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://cxm.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jyy.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tgw.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gef.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qov.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ecw.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hpw.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ydb.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rtb.ydzc1.top

[E15] HTML 转义 / 反转义
来源：http://gld.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://emq.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fcx.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pvx.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bch.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wom.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rwh.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kpc.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmx.tanke756.top

[E16] 数字千分位
来源：http://jxq.hammf.cn

Py:   f"{1234567:,}"
来源：http://gpn.gogol.net.cn

PHP:  number_format(1234567);
来源：http://riu.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://fxa.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qtc.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myc.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cdz.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aav.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://rtv.fzhhl.top

[E17] 首字母大写
来源：http://zkl.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sna.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zhj.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mpj.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fvx.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ous.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://frt.zdbjq.cn

Ruby: s.capitalize
来源：http://ewv.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rwp.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://xjs.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://onw.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kfs.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ycq.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://arc.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oyy.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xbg.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://srq.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xys.xziqi.cn

[E19] 多行文本按行拆分
来源：http://gjr.zhengqikj.top

Py:   s.splitlines()
来源：http://cfs.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://igf.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://ddr.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://wpp.fehbvm.com

Java: s.lines().toList()
来源：http://xtk.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://vjy.cucudq.cn

Ruby: s.lines
来源：http://kzh.yvedp.cn

C#:   s.Split('\n')
来源：http://emy.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://lkv.ydzc1.top

Py:   if not s:
来源：http://api.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fjh.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qxa.nanxuanxn.top

TS:   if (s === "") {}
来源：http://pvu.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://bau.guannengcc.top

Go:   if s == "" {}
来源：http://oib.hongshengwenyu.top

Ruby: if s.empty?
来源：http://mhl.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cms.chenzaomai.com

[E21] 超长截断加省略号
来源：http://gkp.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vmw.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ugh.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsy.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kfg.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nhj.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://lvx.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jdo.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nhb.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://gzk.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zxm.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xaj.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vsg.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://roo.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lkn.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zra.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://azb.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ero.jiagoushi.top

================================================================================
来源：http://ige.ctjpmb.com

F. 文件与目录
来源：http://rho.yueranfly.top

================================================================================
来源：http://qkz.nwbrower.top

[F01] 读取整个文件
来源：http://omi.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://alz.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://vog.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jgh.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fye.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zed.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://shl.sysykeji.top

Ruby: File.read("a.txt")
来源：http://jer.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wls.0kj1m.cn

[F02] 逐行读取文件
来源：http://gsm.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uaq.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cfr.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llg.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lic.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwp.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ose.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pdt.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hwg.ivvv.top

[F03] 写入文件（覆盖）
来源：http://uyh.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdi.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ldz.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fhb.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cgy.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bon.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://opn.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://gmr.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://efs.zhengqikj.top

[F04] 追加写入文件
来源：http://gmh.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://auc.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fqx.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wic.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iix.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ups.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://owa.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://irh.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vdm.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://puo.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://acg.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://mge.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://doe.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://mnx.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://eru.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://arc.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://jsm.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://wkn.guannengcc.top

[F06] 删除文件
来源：http://jwm.nwbrower.top

Py:   os.remove("a.txt")
来源：http://kdl.mhx1999.top

PHP:  unlink("a.txt");
来源：http://duo.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://qsb.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://ufv.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ozw.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://zdf.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://xek.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://ddg.birdmap.top

[F07] 创建目录（含多级）
来源：http://dfn.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tef.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dzz.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://urg.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjl.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oyc.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kho.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fvj.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xfa.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://bei.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://arh.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rio.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://eyd.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://rih.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cxu.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://olj.xinyue.icu

Ruby: Dir.children("dir")
来源：http://cap.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://rin.ctjpmb.com

[F09] 获取文件大小
来源：http://vbe.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://zbw.birdmap.top

PHP:  filesize("a.txt");
来源：http://krg.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://qwt.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://mow.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://lxh.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wke.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://fzy.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://wmu.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://fgn.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vkn.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iye.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kvs.sysykeji.top

TS:   path.extname("a.txt")
来源：http://erz.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iyh.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kms.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ayc.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vbe.yonumen.top

[F11] 复制与移动文件
来源：http://mmw.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jrw.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xuq.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://voc.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bha.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hyp.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jrm.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tca.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mnl.tian-w.cn

[F12] CSV 读写
来源：http://fgm.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dlu.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vxs.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ewk.shuidangran.top

TS:   // 同上
来源：http://szc.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nnv.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfx.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kup.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://irb.chenlongwang.top

================================================================================
来源：http://lzo.xylfe.cn

G. 面向对象
来源：http://hyr.xinyue.icu

================================================================================
来源：http://ate.zhiwuduotai.top

[G01] 定义类
来源：http://jrg.pengpengdd.cyou

Py:   class User: pass
来源：http://iie.daria6918.cn

PHP:  class User {}
来源：http://tgx.nanxinkj.top

JS:   class User {}
来源：http://lyq.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://qel.uphjek.com


<!-- 参考信息 -->