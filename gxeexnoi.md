代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://psi.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gcx.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://exx.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iqd.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ugt.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qhi.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://wgv.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qkv.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lsb.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ilh.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yia.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cvs.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zdd.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aum.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqs.hysaishi.cn

[D26] 数组转字符串
来源：http://yut.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://bob.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://opk.sufxvd.cn

JS:   arr.join(", ")
来源：http://nbr.zhongyouzk.top

TS:   arr.join(", ")
来源：http://cyd.jlsjyb.cn

Java: String.join(", ", list)
来源：http://buq.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://dbx.sufxvd.cn

Ruby: arr.join(", ")
来源：http://idr.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://eby.sxryk.cn

================================================================================
来源：http://ybl.shanyushiyangtech.top

E. 字符串处理
来源：http://osa.tanke756.top

================================================================================
来源：http://pmn.cucudq.cn

[E01] 拼接字符串
来源：http://xna.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uyr.jinghuilouyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sew.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iev.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dkm.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lex.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zog.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sjf.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ndh.dianchejie.cn

[E02] 重复字符串
来源：http://jmz.zhijiandao.cn

Py:   "ab" * 3
来源：http://keg.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://mvw.gzhubu.top

JS:   "ab".repeat(3)
来源：http://aal.guannengcc.top

TS:   "ab".repeat(3)
来源：http://nbc.wangdashe.top

Java: "ab".repeat(3)
来源：http://jwr.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://wbb.hysaishi.cn

Ruby: "ab" * 3
来源：http://wvy.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://isg.kuanghao11.cn

[E03] 截取子串
来源：http://pqc.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgx.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dgy.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wkj.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://xjo.9152youxi.cn

Java: s.substring(1, 4)
来源：http://nll.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qnb.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ydc.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://qdm.nanxuanxn.top

[E04] 查找子串位置
来源：http://pwz.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://zak.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://aip.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pjn.fzhhl.top

TS:   s.indexOf("x")
来源：http://opx.xinyue.icu

Java: s.indexOf("x")
来源：http://aki.sweek.top

Go:   strings.Index(s, "x")
来源：http://hry.guannengcc.top

Ruby: s.index("x")
来源：http://ojv.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://syp.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://tim.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vef.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ooe.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfv.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nmb.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qnz.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wkm.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dim.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://htm.hnxiangtu.top

[E06] 替换子串
来源：http://vfa.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://htu.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://pwu.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lfd.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://vcr.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rom.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fhk.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygp.316326.xyz

C#:   s.Replace("a", "b")
来源：http://zvf.mhx1999.top

[E07] 按分隔符拆分
来源：http://jqq.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qxi.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gln.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://klv.feifeiyinyue.top

TS:   s.split(",")
来源：http://bar.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://rlh.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pxl.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://pgp.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ijt.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://lxg.zhengqikj.top

Py:   ",".join(items)
来源：http://dyg.nwbrower.top

PHP:  implode(",", $items);
来源：http://ueg.jqgufenzy.top

JS:   items.join(",")
来源：http://sfa.nanxuanxn.top

TS:   items.join(",")
来源：http://dce.shzxlz.cn

Java: String.join(",", items)
来源：http://zab.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://xnb.haohaochexian.top

Ruby: items.join(",")
来源：http://wec.aibaodan.cn

C#:   string.Join(",", items)
来源：http://aes.iojbl.cn

[E09] 去除所有空白字符
来源：http://xao.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gpk.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mcb.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://pxh.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://gig.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://ncv.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qwv.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xuk.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://auh.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://vpo.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vbl.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rhh.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://cql.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://nrk.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://uhr.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://elj.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mdq.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bjl.yongpay.top

[E11] 反转字符串
来源：http://dsn.cashguo.top

Py:   s[::-1]
来源：http://zrc.pengpengdd.cyou

PHP:  strrev($s);
来源：http://luw.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://mkn.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://fag.uphjek.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dhz.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://poa.birdmap.top

Ruby: s.reverse
来源：http://zgd.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://gne.epnwcf.com

[E12] 统计某字符出现次数
来源：http://ulb.jinqigfzy.top

Py:   s.count("a")
来源：http://oew.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://tgc.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://xjw.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://yzq.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://prd.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://spl.kuanghao11.cn

Ruby: s.count("a")
来源：http://hnp.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://kdy.xinyue.icu

[E13] 逐字符遍历
来源：http://vin.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://msm.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fzr.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://chi.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gic.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zir.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cdq.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://xqm.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tah.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://igt.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jlg.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rut.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sis.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gdw.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ncz.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qth.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://atx.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lgb.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://yrt.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gwg.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ija.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nmx.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ewh.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vtm.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://upu.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wcz.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://niu.iojbl.cn

[E16] 数字千分位
来源：http://rqq.havefunace.top

Py:   f"{1234567:,}"
来源：http://tih.zdbjq.cn

PHP:  number_format(1234567);
来源：http://xps.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ghv.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hmu.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hul.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lyy.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tdl.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://jqm.ydzc1.top

[E17] 首字母大写
来源：http://qpf.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lxq.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pnv.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nvh.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cse.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vbc.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vxr.yongpay.top

Ruby: s.capitalize
来源：http://raj.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bei.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://qam.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cof.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ibl.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mui.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vib.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uza.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uzh.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sle.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://efm.gzhubu.top

[E19] 多行文本按行拆分
来源：http://fnq.nanxuanxn.top

Py:   s.splitlines()
来源：http://xof.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bdf.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://ift.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://zcv.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://zrx.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://ftz.vqdsnc.cn

Ruby: s.lines
来源：http://hlj.yonumen.top

C#:   s.Split('\n')
来源：http://ufh.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://drq.zhengqikj.top

Py:   if not s:
来源：http://tci.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://agr.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rbz.ydzc1.top

TS:   if (s === "") {}
来源：http://ofk.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://ggn.haohaochexian.top

Go:   if s == "" {}
来源：http://kka.xziqi.cn

Ruby: if s.empty?
来源：http://zvd.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rqu.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://okq.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pok.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ioc.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nlq.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lbd.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vmp.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://ems.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://utg.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jhb.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://xin.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dft.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kvg.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyz.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ydn.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vik.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xxp.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://keg.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://plz.zhoulong.xyz

================================================================================
来源：http://nce.fktsv.cn

F. 文件与目录
来源：http://obd.nanxuanxn.top

================================================================================
来源：http://aqp.yj202588.top

[F01] 读取整个文件
来源：http://amy.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sll.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://oks.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dkd.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vuz.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://lku.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hrj.daxiang520.top

Ruby: File.read("a.txt")
来源：http://hlo.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://ydo.zhongyouzk.top

[F02] 逐行读取文件
来源：http://rwx.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nhp.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://smo.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xuu.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://svs.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://otu.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nop.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://asb.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wfg.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://dgb.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jml.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wrb.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdo.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ewu.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kqr.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://phs.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://och.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zrk.hnxiangtu.top

[F04] 追加写入文件
来源：http://vtx.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qbi.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tui.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bvr.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lnz.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dgu.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvp.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hgo.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zka.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://lnt.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mqw.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://oel.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://cup.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://hbp.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rgb.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://shb.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://jmb.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://kls.hywenlv.cn

[F06] 删除文件
来源：http://yzy.hcnkem.com

Py:   os.remove("a.txt")
来源：http://lwh.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://fwd.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://oiz.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://eqc.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://syf.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://kjb.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://zks.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://qdt.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://fdg.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ney.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ody.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dva.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lcq.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ase.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vtr.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgi.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vmg.sweek.top

[F08] 遍历目录
来源：http://uvt.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lxd.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dfo.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://rwi.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://ryz.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nmg.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cnu.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://piu.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://bxy.zhijiandao.cn


<!-- 参考信息 -->