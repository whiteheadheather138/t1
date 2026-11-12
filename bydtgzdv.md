代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oty.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pgv.cashguo.top

Go:   // 手写循环
来源：http://vzy.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pez.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jbh.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://twh.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wix.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nqr.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fkv.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jlv.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ivi.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lto.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uli.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wdz.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://ngi.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://psm.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wab.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://szd.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eja.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kpe.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dhu.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqf.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ogu.hnxiangtu.top

[D26] 数组转字符串
来源：http://noh.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://xie.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://xyp.zhixingplan.top

JS:   arr.join(", ")
来源：http://ips.kuanghao11.cn

TS:   arr.join(", ")
来源：http://bgq.ehwqpu.com

Java: String.join(", ", list)
来源：http://rsb.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://kjy.iojbl.cn

Ruby: arr.join(", ")
来源：http://wxy.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://rjv.havefunace.top

================================================================================
来源：http://llf.zhixingplan.top

E. 字符串处理
来源：http://kay.gaohongyu789.top

================================================================================
来源：http://qtd.hcnkem.com

[E01] 拼接字符串
来源：http://ulb.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bah.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dco.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bza.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://llk.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ios.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jps.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fhf.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rbs.sxryk.cn

[E02] 重复字符串
来源：http://zdy.havefunace.top

Py:   "ab" * 3
来源：http://vfe.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://uty.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://qcx.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://vhn.shzxlz.cn

Java: "ab".repeat(3)
来源：http://szd.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://bdy.andypj.xyz

Ruby: "ab" * 3
来源：http://sdr.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vql.tanke756.top

[E03] 截取子串
来源：http://oem.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xqg.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://app.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ios.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://iar.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://uqt.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jsf.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hju.ivvv.top

C#:   s.Substring(1, 3)
来源：http://hrv.aibaodan.cn

[E04] 查找子串位置
来源：http://iuw.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://jsj.birdmap.top

PHP:  strpos($s, "x");
来源：http://bqe.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://muy.yangfankeji.com

TS:   s.indexOf("x")
来源：http://bxi.hnxiangtu.top

Java: s.indexOf("x")
来源：http://muz.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://asb.jqgufenzy.top

Ruby: s.index("x")
来源：http://vji.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://jqz.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://irg.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mip.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ong.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kkx.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vmh.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zue.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gpd.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ytx.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yeb.jinqigfzy.top

[E06] 替换子串
来源：http://tqa.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xux.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://oof.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tdq.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://tiu.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ykc.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ehx.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tvd.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://cad.svipenyu.cn

[E07] 按分隔符拆分
来源：http://ntm.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vnd.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pcd.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://btc.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://hjv.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://nxl.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvq.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://xkr.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xaa.meibo888.top

[E08] 数组按分隔符合并
来源：http://ctj.c1oappe.top

Py:   ",".join(items)
来源：http://lqk.bjfxy.top

PHP:  implode(",", $items);
来源：http://jry.zhiwuduotai.top

JS:   items.join(",")
来源：http://tln.xylfe.cn

TS:   items.join(",")
来源：http://skd.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://dmx.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://ybc.xylfe.cn

Ruby: items.join(",")
来源：http://lzg.zhijiandao.cn

C#:   string.Join(",", items)
来源：http://ukx.shuidangran.top

[E09] 去除所有空白字符
来源：http://iqm.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dcr.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kgy.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://bde.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://zae.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://ecz.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://nqy.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://oro.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ior.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://omq.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dxl.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ont.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://egs.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://cee.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://sil.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uiy.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://otf.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sny.cdnleiting.top

[E11] 反转字符串
来源：http://uvw.yuxming.cn

Py:   s[::-1]
来源：http://tgu.xylfe.cn

PHP:  strrev($s);
来源：http://xlj.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://hgq.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://rhi.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://spo.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rvw.andypj.xyz

Ruby: s.reverse
来源：http://six.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://xrq.c1oappe.top

[E12] 统计某字符出现次数
来源：http://quz.chenjidiqi.icu

Py:   s.count("a")
来源：http://vbz.cheryme.top

PHP:  substr_count($s, "a");
来源：http://mji.shuidangran.top

JS:   s.split("a").length - 1
来源：http://iuv.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://eop.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ajo.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://oxe.zhiwuduotai.top

Ruby: s.count("a")
来源：http://poo.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://jdl.yueranfly.top

[E13] 逐字符遍历
来源：http://zyr.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://bfb.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://smv.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xgh.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ffc.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nbl.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mhg.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vxh.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fzc.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://sly.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bjt.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ywv.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rin.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yod.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lzw.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsx.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ang.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://syj.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://lzw.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hbb.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hxd.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fvb.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rpe.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tpo.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rwo.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xkn.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qrm.hfpthk.cn

[E16] 数字千分位
来源：http://twa.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://zjv.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://nwo.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zmc.guannengcc.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jzl.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xha.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gsc.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sfh.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://vch.fanxiaobao.xyz

[E17] 首字母大写
来源：http://hkj.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nyy.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://edy.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bll.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ixo.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://drn.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://llh.haohaochexian.top

Ruby: s.capitalize
来源：http://hip.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zgj.jqgfzy.top

[E18] 模板占位符替换
来源：http://acj.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ffn.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pwu.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ocv.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rhu.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://scr.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mrf.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dgs.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yow.pycfn.com

[E19] 多行文本按行拆分
来源：http://rap.birdmap.top

Py:   s.splitlines()
来源：http://gqi.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kgu.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://sxo.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://duj.ehwqpu.com

Java: s.lines().toList()
来源：http://nso.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://ctv.xinyue.icu

Ruby: s.lines
来源：http://ayg.ctjpmb.com

C#:   s.Split('\n')
来源：http://bpy.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://elu.daxiang520.top

Py:   if not s:
来源：http://vjk.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ktv.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eqc.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://amm.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://qiv.hesvh.cn

Go:   if s == "" {}
来源：http://nhm.ppjwa.cn

Ruby: if s.empty?
来源：http://cwi.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kem.fzhhl.top

[E21] 超长截断加省略号
来源：http://wyy.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ptj.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ldx.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ylh.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhc.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nzp.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://aaj.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cst.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xly.sxryk.cn

[E22] 字节长度与字符长度
来源：http://iwm.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nqd.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xkd.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sks.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://meq.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ccn.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lua.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://mgs.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ulw.jinqigfzy.top

================================================================================
来源：http://phi.fktsv.cn

F. 文件与目录
来源：http://znx.ydzc1.top

================================================================================
来源：http://dqu.hammf.cn

[F01] 读取整个文件
来源：http://hgr.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tsa.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://xam.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zvp.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qha.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://fml.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mdh.fengsongda.top

Ruby: File.read("a.txt")
来源：http://ngv.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://hdp.xuanzx.com

[F02] 逐行读取文件
来源：http://cyl.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vgs.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nqn.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ybd.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://don.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wze.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://peh.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mhp.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dhu.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://uun.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ksi.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bjh.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ewm.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://avi.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oez.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gcr.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://opl.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tqb.zdbjq.cn

[F04] 追加写入文件
来源：http://hlu.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pth.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://llm.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dhk.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://icf.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ucn.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yst.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kdx.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cav.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://kav.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bca.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://ioz.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://woh.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://rqi.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tpl.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lcs.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://ijr.tanke756.top

C#:   File.Exists("a.txt")
来源：http://aiw.vqdsnc.cn

[F06] 删除文件
来源：http://uek.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://fxa.sysykeji.top

PHP:  unlink("a.txt");
来源：http://ngd.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://bty.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vqd.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://duq.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://klx.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://eaw.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://elh.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://oju.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uom.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xkx.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ijz.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwl.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ygd.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lce.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pcx.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://niu.zdbjq.cn

[F08] 遍历目录
来源：http://fjf.316326.xyz


<!-- 参考信息 -->