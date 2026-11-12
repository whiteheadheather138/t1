代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fmt.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vvx.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fmj.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qfp.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mzg.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dpm.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vcy.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://utr.bjfxy.top

[E06] 替换子串
来源：http://mmf.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eki.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://zbi.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mur.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://mgn.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qcc.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qmu.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pja.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://azw.xuanzx.com

[E07] 按分隔符拆分
来源：http://kwh.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ufg.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tba.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fkp.svipenyu.cn

TS:   s.split(",")
来源：http://oqw.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://uhu.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cqh.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://emb.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zen.meibo888.top

[E08] 数组按分隔符合并
来源：http://yyy.yangfankeji.com

Py:   ",".join(items)
来源：http://vwi.yangfankeji.com

PHP:  implode(",", $items);
来源：http://meu.aizwys.cn

JS:   items.join(",")
来源：http://bly.tanke756.top

TS:   items.join(",")
来源：http://aoi.ybcxt.top

Java: String.join(",", items)
来源：http://zlj.guannengcc.top

Go:   strings.Join(items, ",")
来源：http://rfc.ivvv.top

Ruby: items.join(",")
来源：http://oie.iojbl.cn

C#:   string.Join(",", items)
来源：http://vzn.jianghu66.top

[E09] 去除所有空白字符
来源：http://tpm.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://spf.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dpq.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://sbd.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://kuv.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://cxm.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://vpv.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zio.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gih.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://rrv.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xjq.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zxv.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://jos.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://avx.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://ehb.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://the.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tfa.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yug.daxiang520.top

[E11] 反转字符串
来源：http://vtr.bbcook.cn

Py:   s[::-1]
来源：http://jfa.9152youxi.cn

PHP:  strrev($s);
来源：http://law.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://hru.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://kwm.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wwa.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qmo.svipenyu.cn

Ruby: s.reverse
来源：http://sdd.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ixe.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://ilx.bjfxy.top

Py:   s.count("a")
来源：http://wfi.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://xla.shuidangran.top

JS:   s.split("a").length - 1
来源：http://pdq.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://nbo.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fef.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://ufa.sweek.top

Ruby: s.count("a")
来源：http://byf.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://cdh.ydjk.org.cn

[E13] 逐字符遍历
来源：http://fpq.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://vzg.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qin.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mcd.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fhx.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://msg.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nia.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mdv.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eoy.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://luq.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yjb.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfu.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cqc.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://umx.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://evh.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qii.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tmq.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://igl.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://jhj.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://boy.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mls.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jqp.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ejt.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcz.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://npm.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xjp.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jrj.hnqzz.top

[E16] 数字千分位
来源：http://oie.yvedp.cn

Py:   f"{1234567:,}"
来源：http://zko.c1oappe.top

PHP:  number_format(1234567);
来源：http://imt.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://gfz.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://meb.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lms.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jgb.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://amb.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://zrz.zycfv.cn

[E17] 首字母大写
来源：http://ujv.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gsa.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jox.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gor.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cpq.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rgb.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ghl.cqqwz.cn

Ruby: s.capitalize
来源：http://wjq.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vww.fzhhl.top

[E18] 模板占位符替换
来源：http://hvx.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ddc.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mdk.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bph.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tsu.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uri.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://spc.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gkm.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cbe.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://mui.cheryme.top

Py:   s.splitlines()
来源：http://rgt.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xam.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://dhw.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://axc.tianlin.xyz

Java: s.lines().toList()
来源：http://jat.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://hyz.jyoumei.cn

Ruby: s.lines
来源：http://rsl.iojbl.cn

C#:   s.Split('\n')
来源：http://bto.fktsv.cn

[E20] 判断字符串是否为空
来源：http://hki.ywan-chungtsiang.top

Py:   if not s:
来源：http://lwt.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zbc.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hsg.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://xvi.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://qwe.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://fuj.redwolf501.top

Ruby: if s.empty?
来源：http://fsk.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dic.yongpay.top

[E21] 超长截断加省略号
来源：http://tnr.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dul.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rux.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qgf.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztn.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tch.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://kyz.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dgs.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hhj.pycfn.com

[E22] 字节长度与字符长度
来源：http://mve.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jmo.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ccr.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqb.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://avt.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pht.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tmp.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://sbm.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mtu.tanke756.top

================================================================================
来源：http://fiu.yongpay.top

F. 文件与目录
来源：http://skr.ybcxt.top

================================================================================
来源：http://rfd.nwbrower.top

[F01] 读取整个文件
来源：http://bnz.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xso.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://gal.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vmz.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dlc.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zki.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://squ.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://ufo.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://pup.xylfe.cn

[F02] 逐行读取文件
来源：http://elj.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qgt.zhixingplan.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cev.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ing.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iha.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mtd.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ofd.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jng.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mqs.cheryme.top

[F03] 写入文件（覆盖）
来源：http://awg.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://she.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://wqp.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sqm.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbc.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yvc.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://htg.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://odk.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hwa.ppjwa.cn

[F04] 追加写入文件
来源：http://ozc.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mdn.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uio.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvs.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pdf.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://led.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://suv.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wnt.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ltk.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://npf.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tod.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://iln.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://prb.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://cir.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://piz.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hsm.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://kdk.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://oys.tianlin.xyz

[F06] 删除文件
来源：http://jte.cheryme.top

Py:   os.remove("a.txt")
来源：http://xvb.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://uhd.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mbp.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://hxn.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sly.birdmap.top

Go:   os.Remove("a.txt")
来源：http://zsn.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://sep.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://pro.daria6918.cn

[F07] 创建目录（含多级）
来源：http://sgt.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zii.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://arf.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fuz.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aii.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hty.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ojs.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvv.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mgm.jianghu66.top

[F08] 遍历目录
来源：http://ycn.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ezl.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lrl.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://iue.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://dnf.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xaa.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cob.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://dqq.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://viu.sysykeji.top

[F09] 获取文件大小
来源：http://haf.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://fur.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://owx.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://wlm.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://xwg.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rxa.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rcf.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://dlp.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://lsj.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://lve.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://irp.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kxx.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yjp.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://igz.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ljx.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bne.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qyp.cqqwz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qsi.fengsongda.top

[F11] 复制与移动文件
来源：http://ldn.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rvw.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zwo.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qrn.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xus.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://moe.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qfs.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whb.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lyj.dianchejie.cn

[F12] CSV 读写
来源：http://yaj.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xhc.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bnh.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cdl.tianlin.xyz

TS:   // 同上
来源：http://zdy.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xyn.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyb.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ndr.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kna.jinghuilouyu.cn

================================================================================
来源：http://tdb.ybcxt.top

G. 面向对象
来源：http://bdi.yuxming.cn

================================================================================
来源：http://xne.zhengqikj.top

[G01] 定义类
来源：http://owf.chenjidiqi.icu

Py:   class User: pass
来源：http://oqq.gaohongyu789.top

PHP:  class User {}
来源：http://uap.yangfankeji.com

JS:   class User {}
来源：http://gct.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://vaz.nanxinkj.top

Java: class User {}
来源：http://hqy.daxiang520.top

Go:   type User struct { Name string }
来源：http://ssj.cqqwz.cn

Ruby: class User; end
来源：http://nid.shuidangran.top

C#:   class User {}
来源：http://mai.sysykeji.top

[G02] 构造函数
来源：http://ced.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://yho.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://dml.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ytd.tanke756.top

TS:   constructor(public name: string) {}
来源：http://lnm.fanxiaobao.xyz

Java: User(String name) { this.name = name; }
来源：http://vwk.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ywt.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://qug.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://bmk.tian-w.cn

[G03] 实例属性
来源：http://jdo.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://pwy.zycfv.cn

PHP:  public string $name = "x";
来源：http://fht.316326.xyz

JS:   this.name = "x";
来源：http://wae.wangshuangyany.cn

TS:   name: string = "x";
来源：http://xhr.hysaishi.cn

Java: private String name;
来源：http://xtx.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ewk.shzxlz.cn


<!-- 参考信息 -->