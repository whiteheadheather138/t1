代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tbc.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://tdf.wangshuangyany.cn

Py:   Counter(arr)
来源：http://pnt.tanke756.top

PHP:  array_count_values($arr);
来源：http://nxe.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qdv.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gqm.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://biq.hcnkem.com

Go:   // 手写 map[T]int
来源：http://ztn.zhiwuduotai.top

Ruby: arr.tally
来源：http://rgg.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ikk.pycfn.com

[D21] 判断是否包含某元素
来源：http://mqz.kuanghao11.cn

Py:   x in arr
来源：http://knn.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://jgg.fehbvm.com

JS:   arr.includes(x)
来源：http://sik.shuidangran.top

TS:   arr.includes(x)
来源：http://gsg.ivvv.top

Java: list.contains(x)
来源：http://lpi.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://njx.hnqzz.top

Ruby: arr.include?(x)
来源：http://gti.hysaishi.cn

C#:   list.Contains(x)
来源：http://gua.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://gng.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uwq.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://urb.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://acx.mhx1999.top

TS:   [...arr];
来源：http://ocr.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://hhz.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://dcq.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://ubd.kuanghao11.cn

C#:   new List<int>(list);
来源：http://hbo.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://iau.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gpx.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tpz.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qov.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cyq.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zpe.yj20258.top

Go:   // 手写循环
来源：http://pns.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bxj.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vjj.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://aix.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bjq.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://des.yj20258.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xoa.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vym.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zdk.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pwv.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://afb.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mut.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://zmh.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yho.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gvy.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://leu.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cpr.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dme.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://akg.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ipp.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ixn.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://die.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://eon.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://sdp.zhengqikj.top

JS:   arr.join(", ")
来源：http://svv.chenlongwang.top

TS:   arr.join(", ")
来源：http://kuk.jqgfzy.top

Java: String.join(", ", list)
来源：http://vtl.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://zco.guowangkeji.top

Ruby: arr.join(", ")
来源：http://upa.fzhhl.top

C#:   string.Join(", ", list)
来源：http://epo.jyoumei.cn

================================================================================
来源：http://cbl.guannengcc.top

E. 字符串处理
来源：http://hxy.ctjpmb.com

================================================================================
来源：http://bxu.shuidangran.top

[E01] 拼接字符串
来源：http://kdo.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wuf.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ecz.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://syh.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uce.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pvm.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jzz.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hbq.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lco.hysaishi.cn

[E02] 重复字符串
来源：http://wrg.cashguo.top

Py:   "ab" * 3
来源：http://osl.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://wss.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://dol.daxiang520.top

TS:   "ab".repeat(3)
来源：http://nxs.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://uvj.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://lon.havefunace.top

Ruby: "ab" * 3
来源：http://sco.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qvt.gzhubu.top

[E03] 截取子串
来源：http://tkr.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dwz.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hou.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://you.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://jpl.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://aiq.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qcl.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kji.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://gso.tanke756.top

[E04] 查找子串位置
来源：http://wzm.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://qbs.hcnkem.com

PHP:  strpos($s, "x");
来源：http://muu.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hjz.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://ilg.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://uzh.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://rdl.9152youxi.cn

Ruby: s.index("x")
来源：http://xsk.xuanzx.com

C#:   s.IndexOf("x")
来源：http://gem.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nwz.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://odp.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eqw.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pfm.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ona.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zai.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pib.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zwa.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yyk.nwbrower.top

[E06] 替换子串
来源：http://ret.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ukx.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://vmu.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dgg.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://hba.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jnd.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wgt.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ajb.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://fwz.aizwys.cn

[E07] 按分隔符拆分
来源：http://svm.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pcp.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ptw.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://zlx.hammf.cn

TS:   s.split(",")
来源：http://jrk.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://aga.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rsy.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://sbx.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyh.hnqzz.top

[E08] 数组按分隔符合并
来源：http://xwl.nanxuanxn.top

Py:   ",".join(items)
来源：http://yrt.wangdashe.top

PHP:  implode(",", $items);
来源：http://fzg.redwolf501.top

JS:   items.join(",")
来源：http://gif.jinghuilouyu.cn

TS:   items.join(",")
来源：http://fwi.xinyue.icu

Java: String.join(",", items)
来源：http://tqj.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://jcv.yuanzhike.top

Ruby: items.join(",")
来源：http://wgh.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://lzg.ivvv.top

[E09] 去除所有空白字符
来源：http://esr.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tyr.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uea.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://zls.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://gbi.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://yez.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iox.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://irh.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bow.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://vkb.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sot.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fcn.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://oyg.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://ddl.tarul.cn

Java: String.format("%03d", 7)
来源：http://ggv.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aqd.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zzs.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cjn.cheryme.top

[E11] 反转字符串
来源：http://bpv.aibaodan.cn

Py:   s[::-1]
来源：http://ggo.daxiang520.top

PHP:  strrev($s);
来源：http://uth.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://dru.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://fkl.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vmm.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://buh.jinqigufen.top

Ruby: s.reverse
来源：http://uwh.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tio.daxiang520.top

[E12] 统计某字符出现次数
来源：http://wuf.chenzaomai.com

Py:   s.count("a")
来源：http://ldf.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://hgc.jianghu66.top

JS:   s.split("a").length - 1
来源：http://jpl.fengsongda.top

TS:   s.split("a").length - 1
来源：http://qiv.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jux.birdmap.top

Go:   strings.Count(s, "a")
来源：http://fnm.9152youxi.cn

Ruby: s.count("a")
来源：http://qwz.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://eat.sjlbkw.cn

[E13] 逐字符遍历
来源：http://qni.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://wqp.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xei.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ebv.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eey.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kpm.zycfv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qzt.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bhc.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bpi.havefunace.top

[E14] URL 编码与 Base64
来源：http://vej.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lav.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rug.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gfm.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://efp.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mcp.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xdj.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://osa.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tcl.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://yep.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://asq.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bpu.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://way.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lbp.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pyd.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hlw.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jla.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oxv.zhixingplan.top

[E16] 数字千分位
来源：http://qyz.yj202588.top

Py:   f"{1234567:,}"
来源：http://yns.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://rgh.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sbo.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ghk.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://grg.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jru.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hsd.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://okt.sysykeji.top

[E17] 首字母大写
来源：http://zty.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://irn.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://udu.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ycv.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://not.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mtt.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://spl.ctjpmb.com

Ruby: s.capitalize
来源：http://zfd.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hxj.nwbrower.top

[E18] 模板占位符替换
来源：http://hdz.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://miu.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lgz.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://tsj.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pyo.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dha.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xfv.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rnb.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yww.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://xfz.pengpengdd.cyou

Py:   s.splitlines()
来源：http://jir.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cae.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://cdv.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://zko.shuidangran.top

Java: s.lines().toList()
来源：http://nzk.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://xvs.gzhubu.top

Ruby: s.lines
来源：http://gqu.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://kkx.redwolf501.top

[E20] 判断字符串是否为空
来源：http://pfz.sweek.top

Py:   if not s:
来源：http://ebr.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vrp.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xdu.shzxlz.cn

TS:   if (s === "") {}
来源：http://iuy.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://doi.zhiwuduotai.top

Go:   if s == "" {}
来源：http://uod.epnwcf.com

Ruby: if s.empty?
来源：http://ogc.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tra.316326.xyz

[E21] 超长截断加省略号
来源：http://zmk.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pqy.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fkc.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://plt.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qbv.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zjw.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://uxc.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://msl.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ryi.hammf.cn

[E22] 字节长度与字符长度
来源：http://kqx.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://izn.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eic.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wux.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gdg.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jxz.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cym.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://adn.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://phy.quarkkingdee.top

================================================================================
来源：http://zwj.sweek.top

F. 文件与目录
来源：http://xhx.jinqigufen.top

================================================================================
来源：http://mpz.yj202588.top

[F01] 读取整个文件
来源：http://yfd.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nci.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://vqk.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vnp.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qjm.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://kmn.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vls.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://qra.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://pdb.haohaochexian.top

[F02] 逐行读取文件
来源：http://hcn.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zrl.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ohs.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cva.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://huz.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rko.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://drh.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pdg.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://naq.tarul.cn

[F03] 写入文件（覆盖）
来源：http://euf.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qtf.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://twu.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nce.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fku.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fyw.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ewf.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://reb.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://stc.hywenlv.cn

[F04] 追加写入文件
来源：http://fzj.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kha.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kle.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mvu.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jov.sweek.top


<!-- 参考信息 -->