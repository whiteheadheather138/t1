代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fho.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rfl.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xqa.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xig.xylfe.cn

[E06] 替换子串
来源：http://ziv.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kqv.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://vrx.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://czv.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://yaj.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odh.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ruv.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uvi.havefunace.top

C#:   s.Replace("a", "b")
来源：http://gyz.uphjek.com

[E07] 按分隔符拆分
来源：http://wtz.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dst.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://klh.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://efa.tian-w.cn

TS:   s.split(",")
来源：http://rhk.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://bjd.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yqz.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://yfw.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tko.fktsv.cn

[E08] 数组按分隔符合并
来源：http://mui.pycfn.com

Py:   ",".join(items)
来源：http://lwn.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://xzz.yj20258888.top

JS:   items.join(",")
来源：http://ufl.feifeiyinyue.top

TS:   items.join(",")
来源：http://hnj.uphjek.com

Java: String.join(",", items)
来源：http://frt.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://oyp.hongshengwenyu.top

Ruby: items.join(",")
来源：http://yrb.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://osa.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://fde.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lan.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sza.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://nbp.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://pqw.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://kkl.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://lpv.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://pqw.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dos.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://wta.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xaz.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jfh.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://uoc.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://til.yueranfly.top

Java: String.format("%03d", 7)
来源：http://mvd.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kvf.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ait.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ezt.dashuyun.cn

[E11] 反转字符串
来源：http://xzv.chenlongwang.top

Py:   s[::-1]
来源：http://nhw.svipenyu.cn

PHP:  strrev($s);
来源：http://ouf.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://thd.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://mbw.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qdh.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://pnw.yfazqb.com

Ruby: s.reverse
来源：http://yxw.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://min.xziqi.cn

[E12] 统计某字符出现次数
来源：http://trf.jyoumei.cn

Py:   s.count("a")
来源：http://ehl.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://osk.wangdashe.top

JS:   s.split("a").length - 1
来源：http://rnm.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://vbm.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vsz.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://ixt.nanxinkj.top

Ruby: s.count("a")
来源：http://aci.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://ard.yvedp.cn

[E13] 逐字符遍历
来源：http://gmo.cheryme.top

Py:   for ch in s: print(ch)
来源：http://zrp.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zaq.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rwy.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://owq.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://noc.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ffi.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tlp.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hay.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://cwz.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://arc.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qfp.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gzu.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://luj.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rvj.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hwr.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://igz.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gyd.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://nhe.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wau.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://usd.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ycs.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://edl.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ucd.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yed.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zzr.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://osu.zhijiandao.cn

[E16] 数字千分位
来源：http://hhp.jianghu66.top

Py:   f"{1234567:,}"
来源：http://cpz.yfazqb.com

PHP:  number_format(1234567);
来源：http://uma.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://avn.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bfl.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gfv.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aig.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xzo.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://iij.jianghu66.top

[E17] 首字母大写
来源：http://tmh.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cai.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ppq.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ycg.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kbo.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jyc.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zqy.jqgufenzy.top

Ruby: s.capitalize
来源：http://aud.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pzf.hammf.cn

[E18] 模板占位符替换
来源：http://ibi.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vtr.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iva.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tfg.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iil.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hdj.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nry.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cgs.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zdn.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://qli.xuanzx.com

Py:   s.splitlines()
来源：http://doa.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sog.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://zif.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://zum.andypj.xyz

Java: s.lines().toList()
来源：http://eng.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://ufr.xuetiantiany.cn

Ruby: s.lines
来源：http://pik.jlsjyb.cn

C#:   s.Split('\n')
来源：http://uvu.uphjek.com

[E20] 判断字符串是否为空
来源：http://fxc.andypj.xyz

Py:   if not s:
来源：http://dry.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xwy.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qsk.zhongyouzk.top

TS:   if (s === "") {}
来源：http://qom.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://imc.jyoumei.cn

Go:   if s == "" {}
来源：http://hwg.316326.xyz

Ruby: if s.empty?
来源：http://bim.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qgs.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://mfy.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jyd.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hzp.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oqa.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xmy.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://udj.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://nvl.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ead.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sfx.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://jve.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wvv.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pnb.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://abs.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcy.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fqw.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yim.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://aaf.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bfp.yj20258888.top

================================================================================
来源：http://kyb.andypj.xyz

F. 文件与目录
来源：http://rhi.xziqi.cn

================================================================================
来源：http://yfs.vehdjk.com

[F01] 读取整个文件
来源：http://tzh.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ycg.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://zos.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jcy.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ach.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://deq.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vyy.smart0.xyz

Ruby: File.read("a.txt")
来源：http://ske.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://reo.fengsongda.top

[F02] 逐行读取文件
来源：http://bck.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bmb.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rbg.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nux.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://arq.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fec.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ihl.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lia.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xcm.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://lel.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ifm.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://gig.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzq.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdo.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wfj.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vpj.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://emp.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyj.ydjk.org.cn

[F04] 追加写入文件
来源：http://bzl.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://der.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ezh.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljv.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yye.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zmh.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bie.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sti.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lry.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://rib.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjt.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://nhh.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://fyb.fanxiaobao.xyz

TS:   fs.existsSync("a.txt")
来源：http://mhz.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zgo.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jih.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://xbt.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://sth.wangshuangyany.cn

[F06] 删除文件
来源：http://atd.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://sfq.guannengcc.top

PHP:  unlink("a.txt");
来源：http://ard.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://ops.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://qxj.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://knv.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://drd.hammf.cn

Ruby: File.delete("a.txt")
来源：http://ept.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://jgq.gzhubu.top

[F07] 创建目录（含多级）
来源：http://lvo.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oho.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://glo.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zwy.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqk.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://whw.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ffv.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nmg.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://swn.mhx1999.top

[F08] 遍历目录
来源：http://wcd.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ndn.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qjd.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://exe.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://ola.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cck.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lbh.sweek.top

Ruby: Dir.children("dir")
来源：http://wat.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://wpu.havefunace.top

[F09] 获取文件大小
来源：http://whm.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://giu.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://hps.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://tdk.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://bcz.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://oyk.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://imw.fehbvm.com

Ruby: File.size("a.txt")
来源：http://ewq.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://mqr.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://yuz.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://buc.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dki.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lxs.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://ooe.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oiq.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ilv.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://crv.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cnq.snrcjt.cn

[F11] 复制与移动文件
来源：http://erv.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wpf.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wzi.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://whh.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pkv.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dyj.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ugc.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gau.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hiz.zhiwuduotai.top

[F12] CSV 读写
来源：http://aiy.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tar.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ego.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dmz.dashuyun.cn

TS:   // 同上
来源：http://nox.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qve.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xjh.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://prd.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bry.shzxlz.cn

================================================================================
来源：http://jrm.hcnkem.com

G. 面向对象
来源：http://iow.hesvh.cn

================================================================================
来源：http://ydl.aibaodan.cn

[G01] 定义类
来源：http://dgh.ybcxt.top

Py:   class User: pass
来源：http://sbc.fanxiaobao.xyz

PHP:  class User {}
来源：http://oew.jqgufenzy.top

JS:   class User {}
来源：http://fes.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://hro.snrcjt.cn

Java: class User {}
来源：http://jus.xylfe.cn

Go:   type User struct { Name string }
来源：http://ale.cdnleiting.top

Ruby: class User; end
来源：http://caf.jiagoushi.top

C#:   class User {}
来源：http://kwb.haohaochexian.top

[G02] 构造函数
来源：http://xlr.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://otf.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://yfn.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://xwz.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://mnd.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://rhi.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tla.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://ztz.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://qcr.ydzc1.top

[G03] 实例属性
来源：http://idd.cdnleiting.top

Py:   self.name = "x"
来源：http://zbl.guowangkeji.top

PHP:  public string $name = "x";
来源：http://qqo.mhx1999.top

JS:   this.name = "x";
来源：http://crj.ctjpmb.com

TS:   name: string = "x";
来源：http://pdo.aizwys.cn

Java: private String name;
来源：http://xgp.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xpp.sufxvd.cn

Ruby: @name = "x"
来源：http://uin.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://bnc.zdqjudy.top

[G04] 定义方法
来源：http://akv.cheryme.top

Py:   def greet(self): return self.name
来源：http://chc.tanke756.top


<!-- 参考信息 -->