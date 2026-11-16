代发 wailian999

================================================================================
来源：http://lar.daxiang520.top

E. 字符串处理
来源：http://wag.feifeiyinyue.top

================================================================================
来源：http://qku.smart0.xyz

[E01] 拼接字符串
来源：http://rdm.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://riw.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://myu.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wfi.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfm.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://icj.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zgk.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rrh.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mhw.ctjpmb.com

[E02] 重复字符串
来源：http://tgd.fktsv.cn

Py:   "ab" * 3
来源：http://zhj.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://dlz.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://uko.yuxming.cn

TS:   "ab".repeat(3)
来源：http://gyw.zhixingplan.top

Java: "ab".repeat(3)
来源：http://zhk.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://prv.zdbjq.cn

Ruby: "ab" * 3
来源：http://lss.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lsw.redwolf501.top

[E03] 截取子串
来源：http://pfc.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vyf.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ctw.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xeg.iojbl.cn

TS:   s.slice(1, 4)
来源：http://gub.sxryk.cn

Java: s.substring(1, 4)
来源：http://kwd.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hgw.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uma.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://wxx.xziqi.cn

[E04] 查找子串位置
来源：http://vru.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://emc.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://zio.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khn.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://ixr.kuanghao11.cn

Java: s.indexOf("x")
来源：http://cnf.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://cdb.xuetiantiany.cn

Ruby: s.index("x")
来源：http://dzf.shuidangran.top

C#:   s.IndexOf("x")
来源：http://wyo.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fqu.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rvj.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tjv.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kry.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://udc.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zpd.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nox.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vwh.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ouf.hcnkem.com

[E06] 替换子串
来源：http://hfb.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rpe.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://uxh.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://twq.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://rnk.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sms.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzj.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kfc.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://jgq.tian-w.cn

[E07] 按分隔符拆分
来源：http://ccv.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mya.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://htm.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kkp.hnxiangtu.top

TS:   s.split(",")
来源：http://bsn.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://qem.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xos.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://uww.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hpf.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://agp.shzxlz.cn

Py:   ",".join(items)
来源：http://eyl.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://zuc.ppjwa.cn

JS:   items.join(",")
来源：http://xfc.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://fec.jiagoushi.top

Java: String.join(",", items)
来源：http://gtm.birdmap.top

Go:   strings.Join(items, ",")
来源：http://xfw.bjfxy.top

Ruby: items.join(",")
来源：http://aeb.vehdjk.com

C#:   string.Join(",", items)
来源：http://lkc.cqqwz.cn

[E09] 去除所有空白字符
来源：http://qrg.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bhj.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cdu.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://xqf.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://jmv.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://jdh.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://unf.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://srl.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bwg.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://meo.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://owh.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ump.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://loh.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://hyy.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://pan.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://nbj.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dao.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iss.gogol.net.cn

[E11] 反转字符串
来源：http://xya.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://xcm.jiagoushi.top

PHP:  strrev($s);
来源：http://cqn.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://suv.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://eim.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rlp.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xrm.yuxming.cn

Ruby: s.reverse
来源：http://qls.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://nts.xziqi.cn

[E12] 统计某字符出现次数
来源：http://bjp.epnwcf.com

Py:   s.count("a")
来源：http://duj.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://cwl.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://axa.yfazqb.com

TS:   s.split("a").length - 1
来源：http://txy.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ynn.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://oag.zdbjq.cn

Ruby: s.count("a")
来源：http://mjw.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://zbn.zycfv.cn

[E13] 逐字符遍历
来源：http://lnv.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://yvt.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://och.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fnt.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dvp.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ljx.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://edo.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ovr.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sae.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://tit.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rme.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jel.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://exq.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wcd.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ikf.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cma.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dyq.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lgh.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://gmv.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hor.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ruw.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kzd.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uxh.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qbk.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zti.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jvf.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zrw.yvedp.cn

[E16] 数字千分位
来源：http://ctp.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://jyd.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://gsy.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vjq.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wrm.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uxr.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fkv.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hsc.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://tvo.sjlbkw.cn

[E17] 首字母大写
来源：http://xzd.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dxm.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oja.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqg.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iok.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ryo.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aox.ydjk.org.cn

Ruby: s.capitalize
来源：http://fno.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kfp.fengsongda.top

[E18] 模板占位符替换
来源：http://hra.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pqt.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lhc.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vbv.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wbv.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sef.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tju.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bry.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gmi.bbcook.cn

[E19] 多行文本按行拆分
来源：http://axd.chenzaomai.com

Py:   s.splitlines()
来源：http://uhr.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dle.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://spl.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://dol.zhixingplan.top

Java: s.lines().toList()
来源：http://rbz.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://vpx.hongshengwenyu.top

Ruby: s.lines
来源：http://hxq.iojbl.cn

C#:   s.Split('\n')
来源：http://siw.yj20258888.top

[E20] 判断字符串是否为空
来源：http://wlh.fengsongda.top

Py:   if not s:
来源：http://cdk.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qqf.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oet.zhijiandao.cn

TS:   if (s === "") {}
来源：http://tpm.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://rjw.kuanghao11.cn

Go:   if s == "" {}
来源：http://dkj.yongpay.top

Ruby: if s.empty?
来源：http://kgi.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ycn.smart0.xyz

[E21] 超长截断加省略号
来源：http://nza.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hjp.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ygw.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bru.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yfe.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nqd.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://alj.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://udr.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pfc.fengsongda.top

[E22] 字节长度与字符长度
来源：http://lwl.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kws.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dyw.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lqt.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wqc.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kvl.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qhf.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://zun.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jwl.jinyuanbaomall.cn

================================================================================
来源：http://hno.vehdjk.com

F. 文件与目录
来源：http://gmk.yonumen.top

================================================================================
来源：http://ngs.hcnkem.com

[F01] 读取整个文件
来源：http://ttk.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vqv.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://hxm.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sfc.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nve.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kiy.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hto.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://fjg.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://jkb.jyoumei.cn

[F02] 逐行读取文件
来源：http://tgt.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ghh.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nuf.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubd.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxr.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pds.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ipc.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ndl.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sqj.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://zdi.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tgm.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://abv.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sly.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qiq.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://afi.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nqi.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://sjm.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdt.xuanzx.com

[F04] 追加写入文件
来源：http://hco.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ubc.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://reo.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nnx.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhl.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bse.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pdl.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kxd.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rai.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://vjh.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kwg.ivvv.top

PHP:  file_exists("a.txt");
来源：http://hod.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://gpx.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://vzs.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ocp.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rrm.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://aqz.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://ahu.guannengcc.top

[F06] 删除文件
来源：http://ars.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://sox.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://nwd.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aaw.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://hau.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lkq.birdmap.top

Go:   os.Remove("a.txt")
来源：http://aww.havefunace.top

Ruby: File.delete("a.txt")
来源：http://vzp.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://crd.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://xfx.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fxa.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqe.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hid.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uiz.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vnx.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jtd.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cjk.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ust.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://gal.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://chs.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://skt.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://evi.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://xsc.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cdy.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dwj.andypj.xyz

Ruby: Dir.children("dir")
来源：http://sml.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://uoi.hfpthk.cn

[F09] 获取文件大小
来源：http://qyy.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://lxw.mhx1999.top

PHP:  filesize("a.txt");
来源：http://cti.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://luy.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://mek.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mvx.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oho.xinyue.icu

Ruby: File.size("a.txt")
来源：http://jbu.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://lun.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://uvb.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ssj.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zdt.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://puc.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://jhs.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qsg.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vvp.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dcy.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bgt.ppjwa.cn

[F11] 复制与移动文件
来源：http://fku.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://elf.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vae.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhs.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zzk.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vcr.hammf.cn


<!-- 参考信息 -->