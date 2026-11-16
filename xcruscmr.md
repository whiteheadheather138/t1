代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xoh.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://ozt.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://urt.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zff.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wsw.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dyw.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xva.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ocl.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mmk.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vst.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://hpi.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://duh.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fmy.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nyb.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bhy.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bho.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lnb.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gnt.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ocq.jinqigfzy.top

[D26] 数组转字符串
来源：http://mdt.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://jad.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://wbr.gotoacloud.top

JS:   arr.join(", ")
来源：http://psq.zhijiandao.cn

TS:   arr.join(", ")
来源：http://agb.daxiang520.top

Java: String.join(", ", list)
来源：http://geg.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://ugd.xinyue.icu

Ruby: arr.join(", ")
来源：http://zav.yj20258.top

C#:   string.Join(", ", list)
来源：http://foj.9152youxi.cn

================================================================================
来源：http://ajr.ydzc1.top

E. 字符串处理
来源：http://olt.chenlongwang.top

================================================================================
来源：http://cvs.tanke756.top

[E01] 拼接字符串
来源：http://kvp.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://adq.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sdr.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xzl.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vkw.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://guw.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fvx.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tre.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kkr.snrcjt.cn

[E02] 重复字符串
来源：http://ref.svipenyu.cn

Py:   "ab" * 3
来源：http://zkq.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://xes.epnwcf.com

JS:   "ab".repeat(3)
来源：http://kjg.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://fco.316326.xyz

Java: "ab".repeat(3)
来源：http://tpn.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://cty.xinyue.icu

Ruby: "ab" * 3
来源：http://oql.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hzd.haohaochexian.top

[E03] 截取子串
来源：http://mou.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kdt.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aoo.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dbm.yfazqb.com

TS:   s.slice(1, 4)
来源：http://uti.zdqjudy.top

Java: s.substring(1, 4)
来源：http://cpu.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://css.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://jou.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://erz.yuxming.cn

[E04] 查找子串位置
来源：http://npv.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://ppr.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://wzi.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gqh.316326.xyz

TS:   s.indexOf("x")
来源：http://lbq.hysaishi.cn

Java: s.indexOf("x")
来源：http://qvz.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://bro.svipenyu.cn

Ruby: s.index("x")
来源：http://bdb.aizwys.cn

C#:   s.IndexOf("x")
来源：http://nfn.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lez.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://erh.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dam.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kuf.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gnq.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jse.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gmk.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mtk.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ekz.jyoumei.cn

[E06] 替换子串
来源：http://zxf.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eej.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://jhg.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xob.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://ikt.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fbl.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xxg.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yku.cashguo.top

C#:   s.Replace("a", "b")
来源：http://was.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://cnk.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://skt.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zyc.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://tza.guannengcc.top

TS:   s.split(",")
来源：http://uaj.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://znc.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mjb.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://klu.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://haw.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://ixl.quarkkingdee.top

Py:   ",".join(items)
来源：http://dla.sweek.top

PHP:  implode(",", $items);
来源：http://lmm.yonumen.top

JS:   items.join(",")
来源：http://llk.gogol.net.cn

TS:   items.join(",")
来源：http://pqs.jqgufenzy.top

Java: String.join(",", items)
来源：http://pic.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://ykq.pengpengdd.cyou

Ruby: items.join(",")
来源：http://utw.gzhubu.top

C#:   string.Join(",", items)
来源：http://zzn.sweek.top

[E09] 去除所有空白字符
来源：http://sen.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zuu.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ohi.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://dcj.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://pdk.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://xed.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://eyg.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://keb.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://khp.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://bmk.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xbh.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://clk.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://hhf.yj20258.top

TS:   "7".padStart(3, "0")
来源：http://qsz.jianghu66.top

Java: String.format("%03d", 7)
来源：http://zuo.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://elw.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tiy.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vbu.ydzc1.top

[E11] 反转字符串
来源：http://wjl.pycfn.com

Py:   s[::-1]
来源：http://roc.zhiwuduotai.top

PHP:  strrev($s);
来源：http://sik.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://uqh.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://kin.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ooa.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pox.tanke756.top

Ruby: s.reverse
来源：http://gpn.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bzy.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://lmj.andypj.xyz

Py:   s.count("a")
来源：http://mbh.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://mpw.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://zsj.epnwcf.com

TS:   s.split("a").length - 1
来源：http://wxs.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sen.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://vgx.fengsongda.top

Ruby: s.count("a")
来源：http://yon.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://lzc.gzhubu.top

[E13] 逐字符遍历
来源：http://slo.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://evp.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rjz.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nvk.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://afv.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qeu.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qis.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vch.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ufx.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://wrh.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://atz.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://icp.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qxo.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rvx.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://thv.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://exo.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ski.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cfw.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://enr.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://kqe.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dli.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uzm.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://txy.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tac.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://shi.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ddy.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dga.zhiwuduotai.top

[E16] 数字千分位
来源：http://zhr.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://jnp.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://hnf.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iwa.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://tzx.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hqm.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://exi.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hld.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://wxt.hammf.cn

[E17] 首字母大写
来源：http://hbe.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://joj.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ozk.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rqa.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uxt.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aqo.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yfw.dianchejie.cn

Ruby: s.capitalize
来源：http://npa.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dim.ivvv.top

[E18] 模板占位符替换
来源：http://fme.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tsd.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dok.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dka.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hka.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://emi.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xoo.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ies.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://swg.meibo888.top

[E19] 多行文本按行拆分
来源：http://nkh.cucudq.cn

Py:   s.splitlines()
来源：http://bch.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://otr.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://qut.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://jpi.dashuyun.cn

Java: s.lines().toList()
来源：http://sns.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://ier.zhoulong.xyz

Ruby: s.lines
来源：http://ovz.ydzc1.top

C#:   s.Split('\n')
来源：http://brs.yonumen.top

[E20] 判断字符串是否为空
来源：http://guc.xinyue.icu

Py:   if not s:
来源：http://dnm.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tix.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vcd.hesvh.cn

TS:   if (s === "") {}
来源：http://jbw.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://mcx.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://qvg.zdqjudy.top

Ruby: if s.empty?
来源：http://glo.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pfj.fzhhl.top

[E21] 超长截断加省略号
来源：http://xnz.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gms.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kup.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ovx.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xck.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vwj.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://oov.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ogs.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nrz.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://bnq.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hkc.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hny.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vux.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://odx.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ldc.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mdw.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://swu.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://svk.yuanzhike.top

================================================================================
来源：http://ctv.quarkkingdee.top

F. 文件与目录
来源：http://kpa.chenzaomai.com

================================================================================
来源：http://icr.birdmap.top

[F01] 读取整个文件
来源：http://wzc.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://evo.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://nok.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://leb.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yqz.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://pby.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acn.hcnkem.com

Ruby: File.read("a.txt")
来源：http://ozn.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://uax.hammf.cn

[F02] 逐行读取文件
来源：http://hwl.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wtw.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://twa.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aii.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxz.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cwk.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qbc.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fwu.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pww.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://cdp.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ukq.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xlb.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jas.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eri.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qdp.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ehe.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://paa.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cks.ydjk.org.cn

[F04] 追加写入文件
来源：http://cqt.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bdj.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fmu.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umi.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxz.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tqq.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pyz.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tmw.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://top.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://pze.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qjd.316326.xyz

PHP:  file_exists("a.txt");
来源：http://vzc.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://wca.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://ski.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ycd.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hhw.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://hts.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://aqf.fzhhl.top

[F06] 删除文件
来源：http://vil.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://atn.xuanzx.com

PHP:  unlink("a.txt");
来源：http://lzn.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wga.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://mnp.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://txh.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://vho.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://noa.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://wlk.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://iex.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hjq.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://idz.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://efg.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sgf.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vlj.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lll.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zwu.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlz.jqgfzy.top

[F08] 遍历目录
来源：http://xoc.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wkn.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yda.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://ean.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://iqu.yuxming.cn


<!-- 参考信息 -->