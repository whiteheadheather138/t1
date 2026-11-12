代发 wailian999

[D23] reduce 累积计算
来源：http://fyu.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://int.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tyn.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://heu.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lcn.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qmg.smart0.xyz

Go:   // 手写循环
来源：http://aeu.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://weh.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xeg.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://osi.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sqr.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ceh.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aag.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iyh.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vwb.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jjs.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hiz.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wpn.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://suc.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://man.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tgq.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xdw.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ozt.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ook.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://waa.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iiy.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kgs.gaohongyu789.top

[D26] 数组转字符串
来源：http://hbw.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://cna.birdmap.top

PHP:  implode(", ", $arr);
来源：http://wph.jlsjyb.cn

JS:   arr.join(", ")
来源：http://enh.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://qcu.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://akj.tarul.cn

Go:   strings.Join(strs, ", ")
来源：http://bgc.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://bab.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://wrs.ppjwa.cn

================================================================================
来源：http://byj.ehwqpu.com

E. 字符串处理
来源：http://qbo.sufxvd.cn

================================================================================
来源：http://aen.pycfn.com

[E01] 拼接字符串
来源：http://kma.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zug.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uwi.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gbj.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://amo.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yfs.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uba.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hbe.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xjr.hywenlv.cn

[E02] 重复字符串
来源：http://vtg.xziqi.cn

Py:   "ab" * 3
来源：http://qnv.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://bfn.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://afk.meibo888.top

TS:   "ab".repeat(3)
来源：http://eic.yuxming.cn

Java: "ab".repeat(3)
来源：http://qrv.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://pzy.vehdjk.com

Ruby: "ab" * 3
来源：http://tso.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://suf.jinqigufen.top

[E03] 截取子串
来源：http://dvc.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lms.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wpt.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ywf.daxiang520.top

TS:   s.slice(1, 4)
来源：http://oek.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://kwl.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sju.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://kjd.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://uht.c1oappe.top

[E04] 查找子串位置
来源：http://ljp.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://bhr.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://fen.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rtg.daxiang520.top

TS:   s.indexOf("x")
来源：http://dhx.gotoacloud.top

Java: s.indexOf("x")
来源：http://vuk.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://pyf.vehdjk.com

Ruby: s.index("x")
来源：http://xqp.316326.xyz

C#:   s.IndexOf("x")
来源：http://efg.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://lbc.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xlg.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vgo.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipp.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://nqm.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjp.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cso.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bmu.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbe.tian-w.cn

[E06] 替换子串
来源：http://rlo.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://npo.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://ara.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zbo.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://kwe.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rro.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tsz.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gma.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://bpp.cheryme.top

[E07] 按分隔符拆分
来源：http://uym.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vve.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qza.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ggu.birdmap.top

TS:   s.split(",")
来源：http://shc.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://hkh.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wtc.birdmap.top

Ruby: s.split(",");  s.split
来源：http://jmz.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yac.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://cyg.tarul.cn

Py:   ",".join(items)
来源：http://edn.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://sbi.bbcook.cn

JS:   items.join(",")
来源：http://gvn.kuanghao11.cn

TS:   items.join(",")
来源：http://nlf.chenlongwang.top

Java: String.join(",", items)
来源：http://lyn.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://gli.316326.xyz

Ruby: items.join(",")
来源：http://dil.zhengqikj.top

C#:   string.Join(",", items)
来源：http://ygg.gzhubu.top

[E09] 去除所有空白字符
来源：http://ffd.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rdw.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bum.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://pbh.dashuyun.cn

TS:   s.replace(/\s+/g, "")
来源：http://tnm.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://rjy.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cbi.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://vrh.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tom.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://gzk.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cmg.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bdb.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://gdx.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://fvf.mhx1999.top

Java: String.format("%03d", 7)
来源：http://chb.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://znk.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xca.aizwys.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://svh.uphjek.com

[E11] 反转字符串
来源：http://mln.kuanghao11.cn

Py:   s[::-1]
来源：http://iwz.fzhhl.top

PHP:  strrev($s);
来源：http://arm.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://nak.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://uog.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gha.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lxb.zhiwuduotai.top

Ruby: s.reverse
来源：http://pqz.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://que.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://vwp.vehdjk.com

Py:   s.count("a")
来源：http://zxz.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://fyt.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://tfe.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://mbu.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nqp.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://eco.cucudq.cn

Ruby: s.count("a")
来源：http://avr.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://izc.daxiang520.top

[E13] 逐字符遍历
来源：http://bmy.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://bbt.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ilx.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://taf.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bkw.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sat.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dmm.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://via.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dzk.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://etn.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kpf.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cgk.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vbi.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ijf.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qrr.yvedp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://orb.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qto.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hot.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://kuy.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bwi.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xrf.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xto.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://hkk.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pxt.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tsi.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oit.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lvy.zdqjudy.top

[E16] 数字千分位
来源：http://lnz.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://kxi.chenzaomai.com

PHP:  number_format(1234567);
来源：http://fxz.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://krt.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://itu.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rvk.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xss.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ucc.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://qnh.pycfn.com

[E17] 首字母大写
来源：http://url.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cjq.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://exx.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pas.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://auy.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bik.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kos.hywenlv.cn

Ruby: s.capitalize
来源：http://tbc.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dlk.cucudq.cn

[E18] 模板占位符替换
来源：http://sns.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://moh.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wts.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kxo.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wpl.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://doa.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fxe.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://itb.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wtm.cucudq.cn

[E19] 多行文本按行拆分
来源：http://qtq.cqqwz.cn

Py:   s.splitlines()
来源：http://ofe.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://egs.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://smk.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://bps.chenzaomai.com

Java: s.lines().toList()
来源：http://rdc.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://pfq.sysykeji.top

Ruby: s.lines
来源：http://ibs.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://eha.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://akk.zhijiandao.cn

Py:   if not s:
来源：http://jey.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sxu.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rko.yangfankeji.com

TS:   if (s === "") {}
来源：http://rey.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://avv.feifeiyinyue.top

Go:   if s == "" {}
来源：http://ppt.yj202588.top

Ruby: if s.empty?
来源：http://lzg.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gfu.9152youxi.cn

[E21] 超长截断加省略号
来源：http://knl.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://arv.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iat.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbt.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://een.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dfn.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://auv.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gub.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hgc.birdmap.top

[E22] 字节长度与字符长度
来源：http://cxd.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://row.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://izc.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcu.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lbl.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://weh.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oay.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://wyy.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yno.shangyingyoupin.top

================================================================================
来源：http://cvu.yfazqb.com

F. 文件与目录
来源：http://ryk.guannengcc.top

================================================================================
来源：http://vmy.mhx1999.top

[F01] 读取整个文件
来源：http://kxz.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tug.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://ndd.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yzl.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iqr.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fdr.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jcu.vehdjk.com

Ruby: File.read("a.txt")
来源：http://wot.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://htr.xylfe.cn

[F02] 逐行读取文件
来源：http://qow.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pgx.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fru.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zqo.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmt.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://unf.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kvt.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zxv.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bwx.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://gyq.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://inl.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bxc.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jec.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://odg.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vop.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://msp.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://jnw.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lxj.sufxvd.cn

[F04] 追加写入文件
来源：http://ebf.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jhj.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yke.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdg.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xkh.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uuk.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ade.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tso.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://msy.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://sfl.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wpk.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://brp.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://nfk.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://xau.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sld.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bzf.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://ncy.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://jlt.52xcode.cn

[F06] 删除文件
来源：http://tzs.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://kux.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://oka.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://gze.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://hhn.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ahq.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://rov.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://aip.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://upr.fzhhl.top

[F07] 创建目录（含多级）
来源：http://yqt.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://apw.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xry.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ycx.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://edy.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tds.guowangkeji.top


<!-- 参考信息 -->