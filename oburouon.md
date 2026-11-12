代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cix.bbcook.cn

TS:   s.slice(1, 4)
来源：http://vzr.andypj.xyz

Java: s.substring(1, 4)
来源：http://hus.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://spg.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jwf.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://apm.jyoumei.cn

[E04] 查找子串位置
来源：http://nog.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://glx.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://nat.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tkj.ybcxt.top

TS:   s.indexOf("x")
来源：http://ufu.kuanghao11.cn

Java: s.indexOf("x")
来源：http://hxo.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://riy.tianlin.xyz

Ruby: s.index("x")
来源：http://scz.smart0.xyz

C#:   s.IndexOf("x")
来源：http://fyo.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mrm.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wsh.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ypu.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://squ.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://dek.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egs.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nqc.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rqw.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rbt.sjlbkw.cn

[E06] 替换子串
来源：http://lig.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uae.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://sqe.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bqa.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://sws.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rib.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hmj.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://odx.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://ibx.yuanzhike.top

[E07] 按分隔符拆分
来源：http://ydu.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vih.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wjc.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rzi.fengsongda.top

TS:   s.split(",")
来源：http://zak.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ncr.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bzi.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://wij.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ats.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://pcu.ydzc1.top

Py:   ",".join(items)
来源：http://jmo.cdnleiting.top

PHP:  implode(",", $items);
来源：http://rcf.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://jed.tanke756.top

TS:   items.join(",")
来源：http://bge.yuxming.cn

Java: String.join(",", items)
来源：http://afw.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://khz.wangdashe.top

Ruby: items.join(",")
来源：http://wxd.iojbl.cn

C#:   string.Join(",", items)
来源：http://alm.yangfankeji.com

[E09] 去除所有空白字符
来源：http://lni.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kpd.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kaj.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://vji.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://oij.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://wmb.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wfb.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zgh.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lft.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://gip.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dbb.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://teh.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://mlt.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://vkk.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://mjv.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://wln.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://whq.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xtc.meibo888.top

[E11] 反转字符串
来源：http://raf.svipenyu.cn

Py:   s[::-1]
来源：http://qnp.bjfxy.top

PHP:  strrev($s);
来源：http://fzr.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://uvi.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://rju.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://etn.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gwg.tarul.cn

Ruby: s.reverse
来源：http://xbu.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://noh.cashguo.top

[E12] 统计某字符出现次数
来源：http://bzt.xuetiantiany.cn

Py:   s.count("a")
来源：http://ind.havefunace.top

PHP:  substr_count($s, "a");
来源：http://czq.sxryk.cn

JS:   s.split("a").length - 1
来源：http://msr.xinyue.icu

TS:   s.split("a").length - 1
来源：http://xln.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oqx.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://gei.nwbrower.top

Ruby: s.count("a")
来源：http://voe.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://pvy.snrcjt.cn

[E13] 逐字符遍历
来源：http://ogk.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://pzc.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nai.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qzq.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://naw.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ufk.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uft.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://yff.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://knh.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://kuy.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fsv.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mtv.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gkt.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ixo.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mkm.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nnw.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pdd.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xpr.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://sgp.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fca.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wkj.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fcw.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://kkc.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yha.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jxf.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://npt.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zvy.uphjek.com

[E16] 数字千分位
来源：http://jit.fzhhl.top

Py:   f"{1234567:,}"
来源：http://rqd.52xcode.cn

PHP:  number_format(1234567);
来源：http://tbl.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zqu.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rem.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://crp.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iar.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jbx.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://qyl.yj20258.top

[E17] 首字母大写
来源：http://wwb.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mxu.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yit.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvb.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://paj.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cei.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hkp.yanxiufei.cn

Ruby: s.capitalize
来源：http://yez.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mfy.yanxiufei.cn

[E18] 模板占位符替换
来源：http://qjc.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xri.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ozp.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hnf.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wjf.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dkp.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://efm.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zsr.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qvx.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://xck.yongpay.top

Py:   s.splitlines()
来源：http://ley.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ana.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://cas.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://rmg.9152youxi.cn

Java: s.lines().toList()
来源：http://rpk.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://yrw.wangdashe.top

Ruby: s.lines
来源：http://mor.52xcode.cn

C#:   s.Split('\n')
来源：http://ryn.birdmap.top

[E20] 判断字符串是否为空
来源：http://rob.hesvh.cn

Py:   if not s:
来源：http://vua.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lxb.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iev.cheryme.top

TS:   if (s === "") {}
来源：http://suj.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://dfz.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://ect.hysaishi.cn

Ruby: if s.empty?
来源：http://nrt.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qjm.ybcxt.top

[E21] 超长截断加省略号
来源：http://bpc.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dvh.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://usg.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pmg.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmu.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rop.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://wpo.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sfg.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ydz.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://nft.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ulr.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xsh.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cee.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://erw.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lix.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jpn.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://jub.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jds.daria6918.cn

================================================================================
来源：http://ddd.nanxinkj.top

F. 文件与目录
来源：http://ztq.daxiang520.top

================================================================================
来源：http://tmt.c1oappe.top

[F01] 读取整个文件
来源：http://ack.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sfe.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://hhf.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://spn.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hkl.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hzz.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pvw.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://lse.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://umu.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://wcj.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pci.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjo.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ejo.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tfd.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://exc.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sxr.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyg.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cgr.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://kwv.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vac.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zvk.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nzt.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxn.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ffs.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hpy.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://zhn.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xxl.havefunace.top

[F04] 追加写入文件
来源：http://ung.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://khx.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ouw.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rqo.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jok.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jef.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hga.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://npa.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://url.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://xnq.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pfc.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://xeu.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://cxf.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://ept.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wro.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gjf.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://xgb.hammf.cn

C#:   File.Exists("a.txt")
来源：http://wqn.sweek.top

[F06] 删除文件
来源：http://sst.yj20258.top

Py:   os.remove("a.txt")
来源：http://osi.yonumen.top

PHP:  unlink("a.txt");
来源：http://vcb.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://gxp.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://kwi.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hvs.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://ujo.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://jir.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://izp.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://atz.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iqg.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hzb.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fke.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oti.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fin.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mbv.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aol.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bev.cucudq.cn

[F08] 遍历目录
来源：http://rlz.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dla.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://npg.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://als.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://lvf.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dgc.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mmo.ybcxt.top

Ruby: Dir.children("dir")
来源：http://nvf.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://ggg.zycfv.cn

[F09] 获取文件大小
来源：http://fta.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://hvt.vehdjk.com

PHP:  filesize("a.txt");
来源：http://aok.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://hia.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://mtg.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dkz.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gjn.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://ois.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://qfp.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://arv.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://amw.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eol.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iiv.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://job.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iqv.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qzu.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jig.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qmj.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://vxq.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://onh.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aoq.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jag.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dww.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obi.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hoh.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gqt.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yps.uphjek.com

[F12] CSV 读写
来源：http://tdz.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ext.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eyq.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ejd.zdqjudy.top

TS:   // 同上
来源：http://irr.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://teu.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wud.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jrw.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lwh.jinyuanbaomall.cn

================================================================================
来源：http://qvl.jinyuanbaomall.cn

G. 面向对象
来源：http://qll.cucudq.cn

================================================================================
来源：http://roe.pengpengdd.cyou

[G01] 定义类
来源：http://mxt.sxryk.cn

Py:   class User: pass
来源：http://cdr.316326.xyz

PHP:  class User {}
来源：http://jer.zdbjq.cn

JS:   class User {}
来源：http://aqq.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://dqd.daria6918.cn

Java: class User {}
来源：http://cnk.fzhhl.top

Go:   type User struct { Name string }
来源：http://nyv.jinqigufen.top

Ruby: class User; end
来源：http://hmg.hongshengwenyu.top

C#:   class User {}
来源：http://zrd.svipenyu.cn


<!-- 参考信息 -->