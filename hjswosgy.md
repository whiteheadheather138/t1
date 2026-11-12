代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://faz.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mpi.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xfv.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxp.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://abf.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gtx.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://gfa.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vmx.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nvh.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tox.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jxo.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pbn.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://esx.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sjc.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wjs.ybcxt.top

[D26] 数组转字符串
来源：http://nlo.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://ntm.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://pof.jiagoushi.top

JS:   arr.join(", ")
来源：http://rut.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://htw.jlsjyb.cn

Java: String.join(", ", list)
来源：http://bls.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://eun.hammf.cn

Ruby: arr.join(", ")
来源：http://dqe.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://qdr.snrcjt.cn

================================================================================
来源：http://msd.jinyuanbaomall.cn

E. 字符串处理
来源：http://fmd.chenzaomai.com

================================================================================
来源：http://lrr.chenjidiqi.icu

[E01] 拼接字符串
来源：http://sjw.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lua.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xbz.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mxg.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qrm.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vso.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lua.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wco.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://umx.tianlin.xyz

[E02] 重复字符串
来源：http://gnv.fzhhl.top

Py:   "ab" * 3
来源：http://exl.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://mhx.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://dzl.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://ffe.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://fdt.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://wdp.hysaishi.cn

Ruby: "ab" * 3
来源：http://wlk.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zpe.xuanzx.com

[E03] 截取子串
来源：http://wcx.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dqi.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wnt.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qam.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://cof.tian-w.cn

Java: s.substring(1, 4)
来源：http://uhd.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pny.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://zwm.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://fal.xuanzx.com

[E04] 查找子串位置
来源：http://gao.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://hbh.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://bel.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oba.shzxlz.cn

TS:   s.indexOf("x")
来源：http://dpu.nanxinkj.top

Java: s.indexOf("x")
来源：http://ptj.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://nnh.tian-w.cn

Ruby: s.index("x")
来源：http://ldm.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://gxp.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lrb.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dsj.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nxs.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fti.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xpo.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://brv.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zga.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qmf.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qoj.uphjek.com

[E06] 替换子串
来源：http://sii.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rdm.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://ekv.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mzs.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://imf.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xow.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iyp.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jtv.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://akd.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://ukf.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jyx.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bht.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hmm.sjlbkw.cn

TS:   s.split(",")
来源：http://uhu.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://xgg.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://muj.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://fvo.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jys.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://jlv.zhixingplan.top

Py:   ",".join(items)
来源：http://jwm.ybcxt.top

PHP:  implode(",", $items);
来源：http://tdm.cashguo.top

JS:   items.join(",")
来源：http://rfh.xziqi.cn

TS:   items.join(",")
来源：http://jjt.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://wze.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://lbw.hnxiangtu.top

Ruby: items.join(",")
来源：http://qac.chenlongwang.top

C#:   string.Join(",", items)
来源：http://fxe.aibaodan.cn

[E09] 去除所有空白字符
来源：http://lpc.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pxc.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tdy.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://wlb.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://tyv.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://jen.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xer.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://ltr.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qcc.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://jzq.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xdj.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wwh.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://lgc.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://rfl.havefunace.top

Java: String.format("%03d", 7)
来源：http://uvh.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lgr.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ktk.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://txr.yj20258888.top

[E11] 反转字符串
来源：http://srr.shzxlz.cn

Py:   s[::-1]
来源：http://rza.yangfankeji.com

PHP:  strrev($s);
来源：http://pwc.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://wlp.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://vdj.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://abc.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wjc.yongpay.top

Ruby: s.reverse
来源：http://llk.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://jwz.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://jjq.uphjek.com

Py:   s.count("a")
来源：http://jhu.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://iwo.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://boj.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://szw.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rsy.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://rcw.yangfankeji.com

Ruby: s.count("a")
来源：http://anx.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://ozt.meibo888.top

[E13] 逐字符遍历
来源：http://ffl.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://mlo.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://why.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uju.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://xye.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bfs.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wql.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ift.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ktj.yuxming.cn

[E14] URL 编码与 Base64
来源：http://aot.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wit.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pyg.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yrc.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://isz.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cpu.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ted.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ore.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hcw.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://gwr.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vzu.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://unl.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zjn.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zqp.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://glb.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pqh.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tmo.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://prh.jinqigufen.top

[E16] 数字千分位
来源：http://oan.tarul.cn

Py:   f"{1234567:,}"
来源：http://ydx.cqqwz.cn

PHP:  number_format(1234567);
来源：http://ufr.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cvd.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ojx.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lmd.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://esy.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bbo.cheryme.top

C#:   1234567.ToString("N0")
来源：http://rye.dianchejie.cn

[E17] 首字母大写
来源：http://mfm.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dst.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eyj.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hey.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wue.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eec.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zni.aibaodan.cn

Ruby: s.capitalize
来源：http://mln.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uoy.fktsv.cn

[E18] 模板占位符替换
来源：http://ftu.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggq.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cex.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yez.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://edb.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qdw.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gqs.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bkn.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jeg.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://wsa.fehbvm.com

Py:   s.splitlines()
来源：http://lez.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dxn.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://rjl.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://xgc.vqdsnc.cn

Java: s.lines().toList()
来源：http://gao.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://hxa.ybcxt.top

Ruby: s.lines
来源：http://jyu.bbcook.cn

C#:   s.Split('\n')
来源：http://xtc.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://rvz.vehdjk.com

Py:   if not s:
来源：http://fop.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bqp.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qab.yvedp.cn

TS:   if (s === "") {}
来源：http://ngo.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://hfw.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://tgn.havefunace.top

Ruby: if s.empty?
来源：http://vry.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fvm.pycfn.com

[E21] 超长截断加省略号
来源：http://utr.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://avt.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vdp.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gqa.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gri.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://opf.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://sva.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iqj.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://krs.havefunace.top

[E22] 字节长度与字符长度
来源：http://qvh.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://geq.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nau.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ztl.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ulw.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sxq.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmd.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://nof.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hid.quarkkingdee.top

================================================================================
来源：http://hkk.epnwcf.com

F. 文件与目录
来源：http://zsk.xingfuxueyuan.xyz

================================================================================
来源：http://lky.uphjek.com

[F01] 读取整个文件
来源：http://hyw.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pae.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://pzc.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uls.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zsf.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xvu.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iwy.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://gab.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://mmm.fzhhl.top

[F02] 逐行读取文件
来源：http://wvb.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jhr.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zad.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aox.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://frf.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://djw.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xkj.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ffx.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iir.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://ysa.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ibq.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zri.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdf.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztc.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://miz.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lxc.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://qpi.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wfn.uphjek.com

[F04] 追加写入文件
来源：http://pfo.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bby.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ekl.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qgq.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szp.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ktj.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://moy.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ocq.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gaf.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://apt.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pyd.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://yza.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://hpd.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://aqx.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://foa.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hzs.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://its.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://efm.guannengcc.top

[F06] 删除文件
来源：http://yis.yuxming.cn

Py:   os.remove("a.txt")
来源：http://tvx.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://lkp.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://wha.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://jbl.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ozw.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://xjx.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://pvm.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://lxm.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://uhu.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pza.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ttu.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exn.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkp.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eej.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xdo.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cov.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://huk.meibo888.top

[F08] 遍历目录
来源：http://iju.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rfc.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zly.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://smp.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://afm.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ijk.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jed.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://xax.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://mae.snrcjt.cn


<!-- 参考信息 -->