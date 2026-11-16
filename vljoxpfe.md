代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uae.zhiwuduotai.top

[E03] 截取子串
来源：http://xcf.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eaz.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aez.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aho.yj20258888.top

TS:   s.slice(1, 4)
来源：http://psv.bbcook.cn

Java: s.substring(1, 4)
来源：http://erz.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xih.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://boo.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://hpl.quarkkingdee.top

[E04] 查找子串位置
来源：http://dde.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://zqg.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://rbc.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://owb.9152youxi.cn

TS:   s.indexOf("x")
来源：http://dkq.jianghu66.top

Java: s.indexOf("x")
来源：http://kba.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://mnb.hysaishi.cn

Ruby: s.index("x")
来源：http://xsn.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://tzo.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://frj.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://grp.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ivy.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ejg.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://yfi.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igz.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uyg.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kpy.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qxi.316326.xyz

[E06] 替换子串
来源：http://jar.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hgn.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://kkd.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nhy.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://esx.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hty.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dje.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ykg.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://cgg.jyoumei.cn

[E07] 按分隔符拆分
来源：http://oxe.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zxs.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ens.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xgh.chenlongwang.top

TS:   s.split(",")
来源：http://dnm.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ooj.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kwy.havefunace.top

Ruby: s.split(",");  s.split
来源：http://woc.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kcv.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://vba.yanxiufei.cn

Py:   ",".join(items)
来源：http://kto.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://zic.shuidangran.top

JS:   items.join(",")
来源：http://kgw.andypj.xyz

TS:   items.join(",")
来源：http://dam.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://ktd.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://stb.guannengcc.top

Ruby: items.join(",")
来源：http://aqn.316326.xyz

C#:   string.Join(",", items)
来源：http://yar.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://atu.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://url.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dyr.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://paz.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://nje.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://qgz.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jaq.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://xhe.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ngk.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://bxo.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ujn.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://imp.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://dip.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://pix.jianghu66.top

Java: String.format("%03d", 7)
来源：http://rnj.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lxt.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lak.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mcj.hammf.cn

[E11] 反转字符串
来源：http://ydq.daxiang520.top

Py:   s[::-1]
来源：http://pnt.yonumen.top

PHP:  strrev($s);
来源：http://ryv.yonumen.top

JS:   [...s].reverse().join("")
来源：http://lzi.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://wox.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ydo.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gke.chenlongwang.top

Ruby: s.reverse
来源：http://crz.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://esq.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://qtj.pycfn.com

Py:   s.count("a")
来源：http://naw.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://unp.havefunace.top

JS:   s.split("a").length - 1
来源：http://zua.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://hyr.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://smn.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://ktr.dianchejie.cn

Ruby: s.count("a")
来源：http://vfs.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://tlg.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://zsy.birdmap.top

Py:   for ch in s: print(ch)
来源：http://bzj.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jpm.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oxl.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qmh.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lul.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lax.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cvq.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iks.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://sce.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mkh.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cvk.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jrl.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vbe.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wdh.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lpm.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xxu.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vvo.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://mex.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xtf.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jtn.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blr.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://twq.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qmn.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nmu.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zrt.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jud.nanxinkj.top

[E16] 数字千分位
来源：http://xep.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://ulw.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://lhk.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://omx.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qyl.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mts.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zxd.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jdx.yj202588.top

C#:   1234567.ToString("N0")
来源：http://nry.meibo888.top

[E17] 首字母大写
来源：http://acp.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fil.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oom.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vlt.meibo888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cub.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ysk.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xnt.feifeiyinyue.top

Ruby: s.capitalize
来源：http://xqi.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zty.xziqi.cn

[E18] 模板占位符替换
来源：http://pke.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vgd.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://exk.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://exf.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://msi.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cbl.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://juo.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ulm.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://frq.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://usb.yfazqb.com

Py:   s.splitlines()
来源：http://fzt.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nla.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://ghw.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://lkh.tanke756.top

Java: s.lines().toList()
来源：http://knv.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://bsc.zhiwuduotai.top

Ruby: s.lines
来源：http://yvt.chenlongwang.top

C#:   s.Split('\n')
来源：http://zxt.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://the.fktsv.cn

Py:   if not s:
来源：http://ckx.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xvc.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://klz.hammf.cn

TS:   if (s === "") {}
来源：http://hoo.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://agi.iojbl.cn

Go:   if s == "" {}
来源：http://drv.hywenlv.cn

Ruby: if s.empty?
来源：http://lll.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oyu.hcnkem.com

[E21] 超长截断加省略号
来源：http://krd.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qky.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://npx.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsc.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zit.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ujj.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://efh.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://esk.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nxq.c1oappe.top

[E22] 字节长度与字符长度
来源：http://jxj.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://emd.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgb.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ghh.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kat.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uhl.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lzm.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://thd.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nix.shanyushiyangtech.top

================================================================================
来源：http://why.chenjidiqi.icu

F. 文件与目录
来源：http://qdy.yuanzhike.top

================================================================================
来源：http://pis.gogol.net.cn

[F01] 读取整个文件
来源：http://sbs.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pvz.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://xjw.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ncj.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wrz.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zli.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ygk.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://nbi.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://cik.cdnleiting.top

[F02] 逐行读取文件
来源：http://jph.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zqs.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrr.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dhe.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gbg.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ykb.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://arh.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dqo.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qav.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://kxq.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sgd.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dip.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lub.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yml.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wvo.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hiv.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://kjv.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ntm.jiagoushi.top

[F04] 追加写入文件
来源：http://kel.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bqq.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tds.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bho.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dzn.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zvr.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jrt.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xtf.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ukc.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://vsd.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tqr.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://qcq.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://kuy.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://ndk.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://ldq.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pxo.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://tax.hammf.cn

C#:   File.Exists("a.txt")
来源：http://xno.chenzaomai.com

[F06] 删除文件
来源：http://qjn.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://rlw.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://hwa.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://qkk.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://hih.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yjo.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://jjd.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://hml.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://lng.316326.xyz

[F07] 创建目录（含多级）
来源：http://nrs.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://omf.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lkp.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yfa.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vom.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mev.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zas.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tiu.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sbq.ehwqpu.com

[F08] 遍历目录
来源：http://xyy.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oiq.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bek.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://grd.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://nob.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyv.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fur.hnqzz.top

Ruby: Dir.children("dir")
来源：http://wgq.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://yol.zdbjq.cn

[F09] 获取文件大小
来源：http://vbs.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://rhw.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://mlg.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://fqv.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://fhz.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://zrf.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rwu.epnwcf.com

Ruby: File.size("a.txt")
来源：http://cpy.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://yxb.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://dch.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yqz.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cnm.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ckb.yueranfly.top

TS:   path.extname("a.txt")
来源：http://pcs.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gdw.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hxj.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bzz.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://alo.yfazqb.com

[F11] 复制与移动文件
来源：http://yxy.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wyl.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tfa.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://unb.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eqr.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ogi.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://psu.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hcb.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fyh.yj202588.top

[F12] CSV 读写
来源：http://xps.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hyh.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lrd.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://omg.xuetiantiany.cn

TS:   // 同上
来源：http://uzg.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://khy.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ooi.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://igm.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://orj.sufxvd.cn

================================================================================
来源：http://txh.guowangkeji.top

G. 面向对象
来源：http://fer.zhijiandao.cn

================================================================================
来源：http://grj.tarul.cn

[G01] 定义类
来源：http://gue.zhengqikj.top

Py:   class User: pass
来源：http://pqk.snrcjt.cn

PHP:  class User {}
来源：http://vyi.ehwqpu.com

JS:   class User {}
来源：http://xud.tarul.cn

TS:   class User { name: string = ""; }
来源：http://jkq.daria6918.cn


<!-- 参考信息 -->