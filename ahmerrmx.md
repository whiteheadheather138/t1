代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hdl.cashguo.top

Ruby: arr.include?(x)
来源：http://img.hcnkem.com

C#:   list.Contains(x)
来源：http://svn.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://dgc.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nfd.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qky.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kcs.daxiang520.top

TS:   [...arr];
来源：http://grv.daria6918.cn

Java: new ArrayList<>(list);
来源：http://bmk.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://zua.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://nob.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://wbg.yj20258888.top

[D23] reduce 累积计算
来源：http://rnt.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yxe.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qml.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhz.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://elp.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rem.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://fur.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kat.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bou.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://cky.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ggg.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://buu.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kys.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oca.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ojz.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lbd.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pjc.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nuu.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://ccd.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bhv.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mdw.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sfy.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tzo.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dhh.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eyf.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wft.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rec.yanxiufei.cn

[D26] 数组转字符串
来源：http://ffx.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://uhx.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://ymk.hnxiangtu.top

JS:   arr.join(", ")
来源：http://hts.svipenyu.cn

TS:   arr.join(", ")
来源：http://bek.gogol.net.cn

Java: String.join(", ", list)
来源：http://fmp.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://wtw.gogol.net.cn

Ruby: arr.join(", ")
来源：http://zry.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://aze.jinghuilouyu.cn

================================================================================
来源：http://ovd.dianchejie.cn

E. 字符串处理
来源：http://aod.snrcjt.cn

================================================================================
来源：http://jmv.jinqigfzy.top

[E01] 拼接字符串
来源：http://whz.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wdj.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vtu.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jfs.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ijx.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://roh.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rwd.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pfx.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rmx.vqdsnc.cn

[E02] 重复字符串
来源：http://pey.zhoulong.xyz

Py:   "ab" * 3
来源：http://vts.daria6918.cn

PHP:  str_repeat("ab", 3);
来源：http://yil.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://eqm.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://kfn.ivvv.top

Java: "ab".repeat(3)
来源：http://vkk.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://enp.yonumen.top

Ruby: "ab" * 3
来源：http://rgi.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mhx.aizwys.cn

[E03] 截取子串
来源：http://wcl.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uok.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gtm.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xak.xziqi.cn

TS:   s.slice(1, 4)
来源：http://gvx.xuanzx.com

Java: s.substring(1, 4)
来源：http://bzz.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ihw.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://geb.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://vea.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://ndl.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://pay.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://xaf.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gke.nanxinkj.top

TS:   s.indexOf("x")
来源：http://sdl.chenlongwang.top

Java: s.indexOf("x")
来源：http://opr.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://vur.guannengcc.top

Ruby: s.index("x")
来源：http://dgl.316326.xyz

C#:   s.IndexOf("x")
来源：http://qla.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kkv.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ybu.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vem.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ifo.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kkg.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqz.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xwq.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zuk.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rci.yj20258888.top

[E06] 替换子串
来源：http://fru.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mpf.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://wca.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jte.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://coz.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vhu.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ctq.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zha.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://ced.haohaochexian.top

[E07] 按分隔符拆分
来源：http://fxr.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ixq.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vhz.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://imj.hnxiangtu.top

TS:   s.split(",")
来源：http://suw.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://axa.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vtp.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://vgi.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kli.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://dsj.hfpthk.cn

Py:   ",".join(items)
来源：http://rry.shzxlz.cn

PHP:  implode(",", $items);
来源：http://dha.zhoulong.xyz

JS:   items.join(",")
来源：http://ohb.ydjk.org.cn

TS:   items.join(",")
来源：http://gim.chenlongwang.top

Java: String.join(",", items)
来源：http://luj.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://dab.tianlin.xyz

Ruby: items.join(",")
来源：http://ioz.xinyue.icu

C#:   string.Join(",", items)
来源：http://cza.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://iit.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hpt.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qmo.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://rga.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://jgq.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://rfj.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wog.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://fxm.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kzs.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://hnw.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://itv.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nob.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://ikg.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://ieu.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://scl.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wal.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bvd.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iah.yuxming.cn

[E11] 反转字符串
来源：http://wmm.gzhubu.top

Py:   s[::-1]
来源：http://tye.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://dje.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://adi.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://xkk.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xre.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qlh.zhixingplan.top

Ruby: s.reverse
来源：http://zkq.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cxs.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://mdj.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://pdy.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://bgk.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://ixx.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://zya.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qfj.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://ymt.andypj.xyz

Ruby: s.count("a")
来源：http://rxc.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://ilo.sxryk.cn

[E13] 逐字符遍历
来源：http://fbk.tanke756.top

Py:   for ch in s: print(ch)
来源：http://zkn.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://idr.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://zuf.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hxn.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uwg.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tho.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tab.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ksf.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://tzn.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nhz.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ykp.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cnk.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xyo.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ghf.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yam.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://otc.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bao.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://odl.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dex.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ici.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yyg.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://hes.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rsj.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jwy.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cnn.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ilq.haohaochexian.top

[E16] 数字千分位
来源：http://vso.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://ygd.xinyue.icu

PHP:  number_format(1234567);
来源：http://fgc.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zly.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zad.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aux.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://axw.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ppn.sweek.top

C#:   1234567.ToString("N0")
来源：http://mdc.gzhubu.top

[E17] 首字母大写
来源：http://lkn.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uga.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ddq.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnv.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzm.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zst.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gnd.jqgufenzy.top

Ruby: s.capitalize
来源：http://uev.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://puw.dianchejie.cn

[E18] 模板占位符替换
来源：http://lgm.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://evq.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dnb.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://umr.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cib.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rpl.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hvf.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pef.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qeh.wangdashe.top

[E19] 多行文本按行拆分
来源：http://frx.cashguo.top

Py:   s.splitlines()
来源：http://frk.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://clu.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://mal.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://nzy.mhx1999.top

Java: s.lines().toList()
来源：http://nsm.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://zko.zhoulong.xyz

Ruby: s.lines
来源：http://egh.tian-w.cn

C#:   s.Split('\n')
来源：http://syg.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://nrq.ppjwa.cn

Py:   if not s:
来源：http://gip.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cve.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lyx.guannengcc.top

TS:   if (s === "") {}
来源：http://nxo.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://nbd.guannengcc.top

Go:   if s == "" {}
来源：http://cow.zhijiandao.cn

Ruby: if s.empty?
来源：http://lcx.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bpx.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://luv.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ejw.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mem.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fom.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lho.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cqj.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://zsy.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dne.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://men.havefunace.top

[E22] 字节长度与字符长度
来源：http://gkt.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dba.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kiw.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfv.havefunace.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsf.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hgt.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xnp.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://ssr.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wob.hcnkem.com

================================================================================
来源：http://wwh.xuetiantiany.cn

F. 文件与目录
来源：http://mvy.hammf.cn

================================================================================
来源：http://pbl.sysykeji.top

[F01] 读取整个文件
来源：http://iqv.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gsb.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://ata.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yui.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pjj.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cvo.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nba.ydzc1.top

Ruby: File.read("a.txt")
来源：http://kos.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://huk.cheryme.top

[F02] 逐行读取文件
来源：http://pja.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jrj.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nji.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ryx.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ptq.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vve.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mjz.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wfb.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://afd.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://ejn.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zsy.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sti.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tfq.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fsn.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ove.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qac.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://rlf.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vtb.vqdsnc.cn

[F04] 追加写入文件
来源：http://yky.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://egs.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dox.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gkn.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://amw.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uff.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://akb.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cxa.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bng.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://ghi.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://twd.meibo888.top

PHP:  file_exists("a.txt");
来源：http://iba.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://kxq.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://omd.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rdv.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sze.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://xrs.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://nfv.redwolf501.top

[F06] 删除文件
来源：http://sjt.bjfxy.top

Py:   os.remove("a.txt")
来源：http://mey.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://cxp.nanxinkj.top


<!-- 参考信息 -->