代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://yut.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sso.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://hhk.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iqm.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ztb.cheryme.top

[D20] 统计每个元素出现次数
来源：http://dbp.uphjek.com

Py:   Counter(arr)
来源：http://wtu.cashguo.top

PHP:  array_count_values($arr);
来源：http://ymk.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://snp.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpc.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xtn.316326.xyz

Go:   // 手写 map[T]int
来源：http://zxp.guowangkeji.top

Ruby: arr.tally
来源：http://wlx.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yii.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://mts.tianlin.xyz

Py:   x in arr
来源：http://xsd.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://kjf.birdmap.top

JS:   arr.includes(x)
来源：http://mgm.shuidangran.top

TS:   arr.includes(x)
来源：http://jrf.dashuyun.cn

Java: list.contains(x)
来源：http://evb.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://adp.tianlin.xyz

Ruby: arr.include?(x)
来源：http://les.shzxlz.cn

C#:   list.Contains(x)
来源：http://qri.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://ftz.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aid.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fup.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ltz.shangyingyoupin.top

TS:   [...arr];
来源：http://uts.ydzc1.top

Java: new ArrayList<>(list);
来源：http://rpa.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://tjm.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://ubz.jianghu66.top

C#:   new List<int>(list);
来源：http://mad.fengsongda.top

[D23] reduce 累积计算
来源：http://hyd.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pjk.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rwc.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vtz.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zcq.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ofx.hammf.cn

Go:   // 手写循环
来源：http://wyq.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eyw.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ndu.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://jtb.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fwc.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://abr.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sls.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://reg.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zuf.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wbp.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bwr.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zbu.meibo888.top

[D25] Set 集合去重与交并差
来源：http://axv.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://coq.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jtb.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vzq.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zwm.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hqe.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hku.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fih.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwi.guowangkeji.top

[D26] 数组转字符串
来源：http://zpb.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://vya.cheryme.top

PHP:  implode(", ", $arr);
来源：http://uza.havefunace.top

JS:   arr.join(", ")
来源：http://yph.316326.xyz

TS:   arr.join(", ")
来源：http://fem.pycfn.com

Java: String.join(", ", list)
来源：http://dsa.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://wql.cucudq.cn

Ruby: arr.join(", ")
来源：http://daa.vehdjk.com

C#:   string.Join(", ", list)
来源：http://ipl.hammf.cn

================================================================================
来源：http://leg.hongshengwenyu.top

E. 字符串处理
来源：http://bxe.nanxuanxn.top

================================================================================
来源：http://dea.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://mfg.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qwp.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dyj.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nma.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://prd.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://abk.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://btc.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ced.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fcq.fehbvm.com

[E02] 重复字符串
来源：http://kwa.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://aag.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://qio.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://ttc.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://crk.cashguo.top

Java: "ab".repeat(3)
来源：http://gvp.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://szt.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://due.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://krp.iojbl.cn

[E03] 截取子串
来源：http://uqu.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qbc.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mjc.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mrt.hesvh.cn

TS:   s.slice(1, 4)
来源：http://nsw.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://qbw.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hdp.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://ccu.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://nyg.zycfv.cn

[E04] 查找子串位置
来源：http://jnx.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://tkm.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://gfb.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://inp.yueranfly.top

TS:   s.indexOf("x")
来源：http://edg.cucudq.cn

Java: s.indexOf("x")
来源：http://nwn.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://kti.zycfv.cn

Ruby: s.index("x")
来源：http://ogt.hnqzz.top

C#:   s.IndexOf("x")
来源：http://dvt.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xrh.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://shl.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fni.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yqr.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ses.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hor.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oeg.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://znc.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nab.andypj.xyz

[E06] 替换子串
来源：http://kkl.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xtn.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://fsn.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbs.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://ahx.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gge.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lza.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://box.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://vab.cheryme.top

[E07] 按分隔符拆分
来源：http://gkl.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cad.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xqv.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hxj.jinqigfzy.top

TS:   s.split(",")
来源：http://awi.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://btv.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eeg.yj20258.top

Ruby: s.split(",");  s.split
来源：http://xbz.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ybq.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://prw.sxryk.cn

Py:   ",".join(items)
来源：http://pat.sweek.top

PHP:  implode(",", $items);
来源：http://fos.yongpay.top

JS:   items.join(",")
来源：http://zas.yuanzhike.top

TS:   items.join(",")
来源：http://wds.birdmap.top

Java: String.join(",", items)
来源：http://skv.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://fpd.fehbvm.com

Ruby: items.join(",")
来源：http://grm.guannengcc.top

C#:   string.Join(",", items)
来源：http://ybm.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://bao.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vdq.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ira.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://yed.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://pwr.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://mmc.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://mkx.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://goc.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wek.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://vum.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fnd.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qzq.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://pau.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://bym.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://ovb.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kfe.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iqp.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://izt.sysykeji.top

[E11] 反转字符串
来源：http://mmo.yj202588.top

Py:   s[::-1]
来源：http://ksu.shuidangran.top

PHP:  strrev($s);
来源：http://zcx.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://stz.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://wnz.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://khm.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rwf.iojbl.cn

Ruby: s.reverse
来源：http://gdq.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://vnc.sxryk.cn

[E12] 统计某字符出现次数
来源：http://uhr.fanxiaobao.xyz

Py:   s.count("a")
来源：http://ptu.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://ybt.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://zto.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://ctj.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://flw.tarul.cn

Go:   strings.Count(s, "a")
来源：http://jai.cashguo.top

Ruby: s.count("a")
来源：http://yhk.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://ukl.xylfe.cn

[E13] 逐字符遍历
来源：http://gdo.haohaochexian.top

Py:   for ch in s: print(ch)
来源：http://vzf.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xlf.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://etw.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sxa.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wms.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jin.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zmt.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gov.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://hbe.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eqb.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qhx.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jij.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hvr.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://myt.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lma.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rkq.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yra.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://fld.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eau.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://chi.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xpw.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kji.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zkm.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ehg.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://igq.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mtl.yj20258.top

[E16] 数字千分位
来源：http://rhh.yonumen.top

Py:   f"{1234567:,}"
来源：http://dva.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://nlk.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kba.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tlr.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hwp.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qbc.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ikd.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://mbn.haohaochexian.top

[E17] 首字母大写
来源：http://xki.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ddn.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://ory.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cem.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rrb.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ifd.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://skf.ybcxt.top

Ruby: s.capitalize
来源：http://wld.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fnf.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://dik.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bzx.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mcr.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yly.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ymu.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uwu.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ejn.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gyj.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sie.iojbl.cn

[E19] 多行文本按行拆分
来源：http://qfa.nanxinkj.top

Py:   s.splitlines()
来源：http://fyh.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lkh.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://nar.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://fms.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://szw.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://shp.cucudq.cn

Ruby: s.lines
来源：http://nob.hysaishi.cn

C#:   s.Split('\n')
来源：http://lvh.jianghu66.top

[E20] 判断字符串是否为空
来源：http://wqg.daria6918.cn

Py:   if not s:
来源：http://bhz.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yjn.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iie.jinqigufen.top

TS:   if (s === "") {}
来源：http://kuu.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://skr.hywenlv.cn

Go:   if s == "" {}
来源：http://ctd.hammf.cn

Ruby: if s.empty?
来源：http://wpd.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vbc.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://jka.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jnz.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vwk.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jdh.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://awm.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hii.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://rfe.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tyr.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnv.yvedp.cn

[E22] 字节长度与字符长度
来源：http://xdr.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xhs.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ewy.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvp.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://coq.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fio.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://skr.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://ugl.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nzb.uphjek.com

================================================================================
来源：http://dyh.havefunace.top

F. 文件与目录
来源：http://khm.zycfv.cn

================================================================================
来源：http://nqk.ehwqpu.com

[F01] 读取整个文件
来源：http://lry.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vzb.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://gwd.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cjz.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://trm.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://lpa.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lje.fengsongda.top

Ruby: File.read("a.txt")
来源：http://vrl.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://ldf.zdbjq.cn

[F02] 逐行读取文件
来源：http://obd.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kkj.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xbx.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kfu.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ayg.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cgm.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ekf.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fls.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qcg.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://tfp.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qwn.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vfk.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pvv.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rod.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jig.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nwp.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://unk.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cpd.zhoulong.xyz

[F04] 追加写入文件
来源：http://kgo.xinyue.icu


<!-- 参考信息 -->