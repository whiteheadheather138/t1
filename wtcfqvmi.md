代发 wailian999

Go:   strings.Index(s, "x")
来源：http://unh.dianchejie.cn

Ruby: s.index("x")
来源：http://moh.uphjek.com

C#:   s.IndexOf("x")
来源：http://dtg.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pow.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mgy.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ptd.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lyi.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vlr.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kmp.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ktr.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hnu.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cqe.jyoumei.cn

[E06] 替换子串
来源：http://qdx.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vgt.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://bfi.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jlb.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://inr.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://whi.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xhi.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wfb.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://ewy.yangfankeji.com

[E07] 按分隔符拆分
来源：http://lrd.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jcg.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ltw.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://wju.zhiwuduotai.top

TS:   s.split(",")
来源：http://iii.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yri.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://txj.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://isc.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cka.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://nzt.zhoulong.xyz

Py:   ",".join(items)
来源：http://mji.bjfxy.top

PHP:  implode(",", $items);
来源：http://ooi.andypj.xyz

JS:   items.join(",")
来源：http://irp.quarkkingdee.top

TS:   items.join(",")
来源：http://hmp.nanxuanxn.top

Java: String.join(",", items)
来源：http://hdu.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://ufn.ydzc1.top

Ruby: items.join(",")
来源：http://khc.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://xke.hywenlv.cn

[E09] 去除所有空白字符
来源：http://vts.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nsd.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cvk.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fmf.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://uay.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://gny.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ecj.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iqj.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eeh.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://vxu.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zqs.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jkj.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://ylm.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://dzr.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://eex.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nue.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mnr.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iqf.cashguo.top

[E11] 反转字符串
来源：http://iom.nanxinkj.top

Py:   s[::-1]
来源：http://vji.ybcxt.top

PHP:  strrev($s);
来源：http://cbu.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://ljl.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://idx.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jas.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cwg.zhongyouzk.top

Ruby: s.reverse
来源：http://xyq.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://nbe.yj202588.top

[E12] 统计某字符出现次数
来源：http://jlo.pycfn.com

Py:   s.count("a")
来源：http://gsx.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://yao.gzhubu.top

JS:   s.split("a").length - 1
来源：http://sds.fzhhl.top

TS:   s.split("a").length - 1
来源：http://mts.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mqz.yongpay.top

Go:   strings.Count(s, "a")
来源：http://kgt.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://lvl.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://iad.xinyue.icu

[E13] 逐字符遍历
来源：http://ttk.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://byr.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hxr.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://psl.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uph.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pfu.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rms.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aoq.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hml.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://zng.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kfd.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yyc.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://toz.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bll.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bpm.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fmm.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wlm.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yqw.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://ogh.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kof.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fjs.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yrr.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://imp.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sra.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ssm.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ikb.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cei.zhongyouzk.top

[E16] 数字千分位
来源：http://dsc.hammf.cn

Py:   f"{1234567:,}"
来源：http://rfj.0kj1m.cn

PHP:  number_format(1234567);
来源：http://xus.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qwr.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wuk.tarul.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gfc.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eqc.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ibz.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://eqi.jinqigufen.top

[E17] 首字母大写
来源：http://dew.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pdh.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://syj.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfi.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fnc.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ntj.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bej.hongshengwenyu.top

Ruby: s.capitalize
来源：http://zre.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lzu.dianchejie.cn

[E18] 模板占位符替换
来源：http://jbv.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ssa.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://edf.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iji.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zqe.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yyg.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jcx.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rld.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jwy.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://eik.hfpthk.cn

Py:   s.splitlines()
来源：http://izs.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qnz.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://chb.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://dcx.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://pdd.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://sbq.jqgfzy.top

Ruby: s.lines
来源：http://apk.guowangkeji.top

C#:   s.Split('\n')
来源：http://xdo.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://slc.nanxinkj.top

Py:   if not s:
来源：http://rda.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nsz.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cli.andypj.xyz

TS:   if (s === "") {}
来源：http://wif.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://cpj.dashuyun.cn

Go:   if s == "" {}
来源：http://irg.tanke756.top

Ruby: if s.empty?
来源：http://pvk.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ccr.yangfankeji.com

[E21] 超长截断加省略号
来源：http://wvj.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ddu.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bke.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cwa.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbl.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://llp.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://fsr.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mgm.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pla.cheryme.top

[E22] 字节长度与字符长度
来源：http://mrk.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qoe.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rwi.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cuj.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rtf.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dxl.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nnw.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://uow.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nfh.yonumen.top

================================================================================
来源：http://gse.zycfv.cn

F. 文件与目录
来源：http://syj.fengsongda.top

================================================================================
来源：http://dtl.dashuyun.cn

[F01] 读取整个文件
来源：http://klk.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eux.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://btq.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://daj.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qkz.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bbx.xingfuxueyuan.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vnk.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://qsn.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://ieb.zhixingplan.top

[F02] 逐行读取文件
来源：http://bhv.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bwu.dianchejie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pzh.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vnq.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxf.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jxq.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://etg.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fwa.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vrg.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://wvj.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://egr.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tie.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ork.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhb.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aob.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bms.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://goz.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ged.cucudq.cn

[F04] 追加写入文件
来源：http://djk.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ezg.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oya.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrt.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xqy.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hda.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gyk.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rpb.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qda.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://oky.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jwi.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://lod.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://ajk.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://kje.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://emv.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wfh.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://zte.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://pwh.jinghuilouyu.cn

[F06] 删除文件
来源：http://dae.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://xjp.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://hdh.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wbv.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nuc.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oop.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://dct.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://gju.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://ths.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://pjj.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ccd.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://juz.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pmx.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cic.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gvt.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zwf.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nvr.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://boc.zycfv.cn

[F08] 遍历目录
来源：http://ozc.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qvq.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xkv.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://xwy.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://icl.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pji.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wcd.xylfe.cn

Ruby: Dir.children("dir")
来源：http://upi.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://tdy.zhengqikj.top

[F09] 获取文件大小
来源：http://sgp.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://gph.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://yaa.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://bma.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://ory.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fwi.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lar.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://vyn.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://hyp.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://eqs.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://trh.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sqt.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zfx.fktsv.cn

TS:   path.extname("a.txt")
来源：http://kfi.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sat.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pdn.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yto.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ibq.haohaochexian.top

[F11] 复制与移动文件
来源：http://tia.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jva.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fbn.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjl.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://feo.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ybq.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vpn.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqe.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dqg.xuetiantiany.cn

[F12] CSV 读写
来源：http://irg.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://auv.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nsm.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zhf.vqdsnc.cn

TS:   // 同上
来源：http://sfz.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fjs.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hiq.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xoe.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sdj.shuidangran.top

================================================================================
来源：http://cbb.hnqzz.top

G. 面向对象
来源：http://rti.uphjek.com

================================================================================
来源：http://uzh.xziqi.cn

[G01] 定义类
来源：http://kdy.cqqwz.cn

Py:   class User: pass
来源：http://rro.fktsv.cn

PHP:  class User {}
来源：http://zky.yfazqb.com

JS:   class User {}
来源：http://dis.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://dil.ehwqpu.com

Java: class User {}
来源：http://pod.52xcode.cn

Go:   type User struct { Name string }
来源：http://vfp.zhijiandao.cn

Ruby: class User; end
来源：http://xnb.pengpengdd.cyou

C#:   class User {}
来源：http://qva.dianchejie.cn

[G02] 构造函数
来源：http://gbd.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://ion.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://xdh.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://pqo.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://utr.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://jev.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hbo.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://bwd.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://zbf.yueranfly.top

[G03] 实例属性
来源：http://yig.ivvv.top

Py:   self.name = "x"
来源：http://kvh.shuidangran.top

PHP:  public string $name = "x";
来源：http://njp.xuetiantiany.cn


<!-- 参考信息 -->