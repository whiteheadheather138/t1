代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cdo.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gby.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ddq.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uqg.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysk.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tac.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pdd.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://txm.fktsv.cn

[E06] 替换子串
来源：http://rty.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cix.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://jho.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vdd.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://pcx.hesvh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gun.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wst.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pon.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://fws.redwolf501.top

[E07] 按分隔符拆分
来源：http://xkt.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://unv.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rjp.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xfv.tanke756.top

TS:   s.split(",")
来源：http://qpb.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ekd.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ebf.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://dnv.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jbv.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://xqy.c1oappe.top

Py:   ",".join(items)
来源：http://scp.xuanzx.com

PHP:  implode(",", $items);
来源：http://rxn.havefunace.top

JS:   items.join(",")
来源：http://vqh.chenjidiqi.icu

TS:   items.join(",")
来源：http://twa.hongshengwenyu.top

Java: String.join(",", items)
来源：http://ebx.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://twe.ctjpmb.com

Ruby: items.join(",")
来源：http://twi.dianchejie.cn

C#:   string.Join(",", items)
来源：http://qan.xinyue.icu

[E09] 去除所有空白字符
来源：http://uvk.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rpm.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dne.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://ktv.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://ogo.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://lnt.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://omw.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://khf.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nrv.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://blc.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kne.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sgz.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://wmt.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://ren.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://ksd.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yha.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ilz.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ayc.fehbvm.com

[E11] 反转字符串
来源：http://nlx.cdnleiting.top

Py:   s[::-1]
来源：http://raf.zdqjudy.top

PHP:  strrev($s);
来源：http://ryz.tanke756.top

JS:   [...s].reverse().join("")
来源：http://pam.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://vux.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hta.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ouy.yanxiufei.cn

Ruby: s.reverse
来源：http://dzb.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://qdk.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://asm.gotoacloud.top

Py:   s.count("a")
来源：http://ejo.havefunace.top

PHP:  substr_count($s, "a");
来源：http://byd.shuidangran.top

JS:   s.split("a").length - 1
来源：http://vvk.wangdashe.top

TS:   s.split("a").length - 1
来源：http://wrc.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kje.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://zry.kuanghao11.cn

Ruby: s.count("a")
来源：http://vnb.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://rkb.zdbjq.cn

[E13] 逐字符遍历
来源：http://jma.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://ofv.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmr.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jll.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fwy.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gif.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kab.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://dli.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fpa.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://wbq.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sxn.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://odw.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wnt.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mtg.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mab.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gwj.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oas.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://smq.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://fzg.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kdp.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wfx.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ybm.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://foh.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://alg.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://req.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ige.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eky.andypj.xyz

[E16] 数字千分位
来源：http://rqt.daria6918.cn

Py:   f"{1234567:,}"
来源：http://nte.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://znh.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://svb.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hqt.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cna.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fxq.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fye.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://bln.tianlin.xyz

[E17] 首字母大写
来源：http://jpv.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rez.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://isk.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ntn.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kds.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gxt.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dsy.sjlbkw.cn

Ruby: s.capitalize
来源：http://zpx.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojy.yonumen.top

[E18] 模板占位符替换
来源：http://oxb.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kxy.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gii.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bjg.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nag.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qax.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qfc.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aby.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://msh.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://siy.cheryme.top

Py:   s.splitlines()
来源：http://ava.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zur.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://tbe.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://mfu.jinqigufen.top

Java: s.lines().toList()
来源：http://ery.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://cff.fktsv.cn

Ruby: s.lines
来源：http://yvt.cheryme.top

C#:   s.Split('\n')
来源：http://jfl.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://ede.kuanghao11.cn

Py:   if not s:
来源：http://foj.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://quo.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rck.0kj1m.cn

TS:   if (s === "") {}
来源：http://jke.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://lwm.kuanghao11.cn

Go:   if s == "" {}
来源：http://fax.zdbjq.cn

Ruby: if s.empty?
来源：http://ncy.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jqi.yfazqb.com

[E21] 超长截断加省略号
来源：http://jua.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aok.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jnm.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ozz.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sbe.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://toc.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://pms.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ghh.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jim.guowangkeji.top

[E22] 字节长度与字符长度
来源：http://zyh.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kji.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sxx.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://drw.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://anm.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://faj.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://svq.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://hhj.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fjz.hcnkem.com

================================================================================
来源：http://xqw.jiagoushi.top

F. 文件与目录
来源：http://eiw.nanxuanxn.top

================================================================================
来源：http://aci.jianghu66.top

[F01] 读取整个文件
来源：http://oxw.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://glm.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://osa.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ayh.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://luo.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ibm.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://azq.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://cug.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://mbo.jqgufenzy.top

[F02] 逐行读取文件
来源：http://zaf.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uij.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lvv.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zla.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zyy.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zeg.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eeu.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mkc.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ozp.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://myg.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hyl.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://aak.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgf.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rde.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iph.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jns.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://bbk.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ife.iojbl.cn

[F04] 追加写入文件
来源：http://acy.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zyb.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://clf.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nmk.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qmc.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bfu.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nxx.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mgf.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://afr.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://rta.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qiq.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://exo.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://gdj.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://ava.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dca.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qkz.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://cjo.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://zas.hfpthk.cn

[F06] 删除文件
来源：http://tas.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://hyi.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://yzv.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dbo.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://rzx.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oub.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://rwi.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://hpz.yongpay.top

C#:   File.Delete("a.txt");
来源：http://tgq.aizwys.cn

[F07] 创建目录（含多级）
来源：http://dog.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mgg.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eki.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndz.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rkf.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ntp.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dlp.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bcx.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nem.yj20258.top

[F08] 遍历目录
来源：http://dgn.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://yoq.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vvc.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://ctv.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://onz.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fcx.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://rfw.xingfuxueyuan.xyz

Ruby: Dir.children("dir")
来源：http://zko.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://xaw.fengsongda.top

[F09] 获取文件大小
来源：http://dbd.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://stv.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://khh.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://usk.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://wlx.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://qpc.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vrf.shuidangran.top

Ruby: File.size("a.txt")
来源：http://igc.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://jcm.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://aog.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pwq.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://frs.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cpy.sxryk.cn

TS:   path.extname("a.txt")
来源：http://ujx.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afg.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pxp.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vvt.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bzy.zhixingplan.top

[F11] 复制与移动文件
来源：http://owu.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vsa.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fnt.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcz.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mal.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uqh.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://euc.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://spc.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mvy.hysaishi.cn

[F12] CSV 读写
来源：http://uoa.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://itr.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hqm.yj20258888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://odm.shanyushiyangtech.top

TS:   // 同上
来源：http://qfw.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ptv.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vfi.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hge.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fkq.yuanzhike.top

================================================================================
来源：http://ndr.dianchejie.cn

G. 面向对象
来源：http://gxe.vqdsnc.cn

================================================================================
来源：http://ayg.ctjpmb.com

[G01] 定义类
来源：http://gok.jinqigfzy.top

Py:   class User: pass
来源：http://mwm.vehdjk.com

PHP:  class User {}
来源：http://vzi.sysykeji.top

JS:   class User {}
来源：http://hnb.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://vmu.yanxiufei.cn

Java: class User {}
来源：http://wwi.fktsv.cn

Go:   type User struct { Name string }
来源：http://wmv.52xcode.cn

Ruby: class User; end
来源：http://zuo.svipenyu.cn

C#:   class User {}
来源：http://mud.jinghuilouyu.cn

[G02] 构造函数
来源：http://jwk.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://awk.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://hmo.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://ehn.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://jwk.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://teg.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wyi.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://dhc.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://unz.xinyue.icu

[G03] 实例属性
来源：http://wrh.xinyue.icu

Py:   self.name = "x"
来源：http://ovp.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://ylz.snrcjt.cn

JS:   this.name = "x";
来源：http://rtv.zhengqikj.top

TS:   name: string = "x";
来源：http://aea.zhaomingkeji.xyz

Java: private String name;
来源：http://sxx.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nrz.cucudq.cn


<!-- 参考信息 -->