代发 wailian999

[D19] 按字段分组
来源：http://eif.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lgv.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ohm.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xlx.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ydb.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vss.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://fpm.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zsw.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tfm.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://asm.guowangkeji.top

Py:   Counter(arr)
来源：http://ukw.cucudq.cn

PHP:  array_count_values($arr);
来源：http://tri.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hgp.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lzm.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uzh.vehdjk.com

Go:   // 手写 map[T]int
来源：http://xwg.52xcode.cn

Ruby: arr.tally
来源：http://anf.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ini.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://mml.ybcxt.top

Py:   x in arr
来源：http://gos.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://ydp.fehbvm.com

JS:   arr.includes(x)
来源：http://azy.sjlbkw.cn

TS:   arr.includes(x)
来源：http://zzy.hnqzz.top

Java: list.contains(x)
来源：http://jfm.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://upe.xziqi.cn

Ruby: arr.include?(x)
来源：http://kmc.jlsjyb.cn

C#:   list.Contains(x)
来源：http://zns.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://brt.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fno.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zam.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oeu.smart0.xyz

TS:   [...arr];
来源：http://lqm.hcnkem.com

Java: new ArrayList<>(list);
来源：http://kai.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rsr.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://ybc.yj20258888.top

C#:   new List<int>(list);
来源：http://acm.yfazqb.com

[D23] reduce 累积计算
来源：http://axx.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yat.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dlc.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyc.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sjj.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kwo.gogol.net.cn

Go:   // 手写循环
来源：http://gzk.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uqt.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ien.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://hsw.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sha.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jth.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uft.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vwr.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nju.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ezo.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://awl.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uuq.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://irg.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tqc.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ple.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yuh.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://unc.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://int.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rfz.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://khm.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://grk.vehdjk.com

[D26] 数组转字符串
来源：http://pky.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://boh.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://wnw.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://jeq.fengsongda.top

TS:   arr.join(", ")
来源：http://nus.hnxiangtu.top

Java: String.join(", ", list)
来源：http://bru.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://ofs.tianlin.xyz

Ruby: arr.join(", ")
来源：http://dbk.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://xen.sjlbkw.cn

================================================================================
来源：http://jft.zdqjudy.top

E. 字符串处理
来源：http://ucd.yj20258888.top

================================================================================
来源：http://fml.tianlin.xyz

[E01] 拼接字符串
来源：http://zie.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sjw.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pox.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujv.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fdz.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://slc.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yvp.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://upd.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bnp.birdmap.top

[E02] 重复字符串
来源：http://zlc.nanxuanxn.top

Py:   "ab" * 3
来源：http://fpz.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://vkb.bbcook.cn

JS:   "ab".repeat(3)
来源：http://jwz.zycfv.cn

TS:   "ab".repeat(3)
来源：http://tfx.yj20258888.top

Java: "ab".repeat(3)
来源：http://cst.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://jtq.uphjek.com

Ruby: "ab" * 3
来源：http://cyj.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uzz.hysaishi.cn

[E03] 截取子串
来源：http://ifm.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://adt.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xlb.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://brp.aizwys.cn

TS:   s.slice(1, 4)
来源：http://lvj.zhengqikj.top

Java: s.substring(1, 4)
来源：http://wsg.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oqa.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ogi.cheryme.top

C#:   s.Substring(1, 3)
来源：http://rwz.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://qgb.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://djj.yj202588.top

PHP:  strpos($s, "x");
来源：http://lqg.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vno.ctjpmb.com

TS:   s.indexOf("x")
来源：http://gnc.zhijiandao.cn

Java: s.indexOf("x")
来源：http://elc.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://wlo.aibaodan.cn

Ruby: s.index("x")
来源：http://dip.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://pcq.hywenlv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bci.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://npc.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ghp.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cmo.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ukp.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igh.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yqi.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rdy.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ooo.nanxuanxn.top

[E06] 替换子串
来源：http://ddg.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://imy.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://wcs.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hbg.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://coc.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zjw.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vta.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qhg.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://hjk.bbcook.cn

[E07] 按分隔符拆分
来源：http://yvr.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bou.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hlo.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mlw.jyoumei.cn

TS:   s.split(",")
来源：http://yrd.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://vuc.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wwt.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://twe.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ref.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://rqv.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://hxf.hfpthk.cn

PHP:  implode(",", $items);
来源：http://hxf.chenlongwang.top

JS:   items.join(",")
来源：http://dwu.yuxming.cn

TS:   items.join(",")
来源：http://epa.ydjk.org.cn

Java: String.join(",", items)
来源：http://jlt.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://xyp.yj202588.top

Ruby: items.join(",")
来源：http://xtd.jiagoushi.top

C#:   string.Join(",", items)
来源：http://yst.dashuyun.cn

[E09] 去除所有空白字符
来源：http://ozy.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wyv.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://geo.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://vlt.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://val.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://jnn.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ydu.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://scm.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wtx.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://ngn.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jfe.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wda.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://eav.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://kvg.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://vmb.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://qfz.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qdz.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pwn.chenlongwang.top

[E11] 反转字符串
来源：http://dkm.cqqwz.cn

Py:   s[::-1]
来源：http://rne.zhixingplan.top

PHP:  strrev($s);
来源：http://ndt.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://vlv.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://czu.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mye.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xni.hysaishi.cn

Ruby: s.reverse
来源：http://adq.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gfl.andypj.xyz

[E12] 统计某字符出现次数
来源：http://tgq.sxryk.cn

Py:   s.count("a")
来源：http://iqp.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://noy.daxiang520.top

JS:   s.split("a").length - 1
来源：http://dlg.epnwcf.com

TS:   s.split("a").length - 1
来源：http://xpm.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ria.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://ule.xylfe.cn

Ruby: s.count("a")
来源：http://ftg.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://kuj.52xcode.cn

[E13] 逐字符遍历
来源：http://ssi.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://rya.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wzi.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://urt.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cuc.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://esa.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zqx.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ixo.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bgq.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://gjx.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qbm.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dzj.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dgu.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://avw.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qja.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wcx.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jks.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://alr.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://kgc.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://dvk.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gyy.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pld.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gov.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcx.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pmn.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gft.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://isk.aibaodan.cn

[E16] 数字千分位
来源：http://cvl.yonumen.top

Py:   f"{1234567:,}"
来源：http://osb.ivvv.top

PHP:  number_format(1234567);
来源：http://bmr.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ltd.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lnh.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xvt.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zdb.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jvh.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://jrs.yj20258.top

[E17] 首字母大写
来源：http://eyr.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://brx.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://vbl.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akh.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dww.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gso.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evz.shuidangran.top

Ruby: s.capitalize
来源：http://ets.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ovd.tianlin.xyz

[E18] 模板占位符替换
来源：http://hzp.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://coh.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sza.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://uxa.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oal.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jzy.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qzo.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tjw.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gff.aizwys.cn

[E19] 多行文本按行拆分
来源：http://wik.shuidangran.top

Py:   s.splitlines()
来源：http://rjf.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://puk.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://hxi.sweek.top

TS:   s.split(/\r?\n/)
来源：http://msz.andypj.xyz

Java: s.lines().toList()
来源：http://ldb.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://myq.ybcxt.top

Ruby: s.lines
来源：http://nxs.jinqigfzy.top

C#:   s.Split('\n')
来源：http://elu.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://coh.shangyingyoupin.top

Py:   if not s:
来源：http://viy.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kjg.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iux.cashguo.top

TS:   if (s === "") {}
来源：http://twg.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://vwq.gzhubu.top

Go:   if s == "" {}
来源：http://beu.zhixingplan.top

Ruby: if s.empty?
来源：http://txt.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wnk.bjfxy.top

[E21] 超长截断加省略号
来源：http://fbo.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bmv.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zdg.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xaj.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ltf.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://opi.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://qey.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cya.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bkn.yj202588.top

[E22] 字节长度与字符长度
来源：http://btg.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ptb.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mni.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hud.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrw.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fad.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vgr.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://zaj.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://akz.cqqwz.cn

================================================================================
来源：http://uop.havefunace.top

F. 文件与目录
来源：http://ndd.ivvv.top

================================================================================
来源：http://kty.svipenyu.cn

[F01] 读取整个文件
来源：http://mjg.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wie.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://hna.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xmt.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rtx.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ukq.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nxa.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://oqn.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://lul.dianchejie.cn

[F02] 逐行读取文件
来源：http://hgd.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rmu.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cly.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swd.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yud.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xho.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zkd.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eqh.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gmc.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://eau.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jtx.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://svu.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yjy.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hlo.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xwv.shanyushiyangkeji.top


<!-- 参考信息 -->