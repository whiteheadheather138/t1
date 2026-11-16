代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://grc.tian-w.cn

Go:   // 手写双层循环
来源：http://xqm.ehwqpu.com

Ruby: nested.flatten
来源：http://gll.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jvj.hongshengwenyu.top

[D19] 按字段分组
来源：http://gnl.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://srl.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gjn.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://get.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cny.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ogp.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://okd.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ktp.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://crn.ivvv.top

[D20] 统计每个元素出现次数
来源：http://vgn.jiagoushi.top

Py:   Counter(arr)
来源：http://jvx.birdmap.top

PHP:  array_count_values($arr);
来源：http://ban.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yko.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwe.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eyl.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://yap.kuanghao11.cn

Ruby: arr.tally
来源：http://ufb.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zxq.yonumen.top

[D21] 判断是否包含某元素
来源：http://hnn.tarul.cn

Py:   x in arr
来源：http://bfy.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://bfc.bbcook.cn

JS:   arr.includes(x)
来源：http://zbo.shzxlz.cn

TS:   arr.includes(x)
来源：http://dgg.yvedp.cn

Java: list.contains(x)
来源：http://rub.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://fqf.yangfankeji.com

Ruby: arr.include?(x)
来源：http://itt.jlsjyb.cn

C#:   list.Contains(x)
来源：http://cno.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://fhj.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jrv.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xbe.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cku.316326.xyz

TS:   [...arr];
来源：http://reo.fengsongda.top

Java: new ArrayList<>(list);
来源：http://okm.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://joz.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://rtu.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://zgz.vehdjk.com

[D23] reduce 累积计算
来源：http://fpv.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xre.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jxj.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jem.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kwz.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jze.yongpay.top

Go:   // 手写循环
来源：http://nye.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://brw.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dft.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://njt.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://smg.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://usk.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jsd.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bkq.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zrr.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ska.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mam.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mpk.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://qbe.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xlo.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wla.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://odq.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gps.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fpb.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wny.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ltg.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pom.tianlin.xyz

[D26] 数组转字符串
来源：http://xdu.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://nrj.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://zmj.ehwqpu.com

JS:   arr.join(", ")
来源：http://jhh.dianchejie.cn

TS:   arr.join(", ")
来源：http://cwd.yuanzhike.top

Java: String.join(", ", list)
来源：http://ixd.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://ezr.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://pdp.c1oappe.top

C#:   string.Join(", ", list)
来源：http://crw.quarkkingdee.top

================================================================================
来源：http://bcy.xuanzx.com

E. 字符串处理
来源：http://vdu.jyoumei.cn

================================================================================
来源：http://ksp.hammf.cn

[E01] 拼接字符串
来源：http://dvy.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kfv.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oif.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nla.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://grw.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://erp.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fmx.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ttx.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uqc.yongpay.top

[E02] 重复字符串
来源：http://hai.yongpay.top

Py:   "ab" * 3
来源：http://zpy.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://kfz.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://flr.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://zpa.hcnkem.com

Java: "ab".repeat(3)
来源：http://obv.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://ycn.shuidangran.top

Ruby: "ab" * 3
来源：http://adw.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mde.cqqwz.cn

[E03] 截取子串
来源：http://hal.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gxp.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jbj.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ojq.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://soh.0kj1m.cn

Java: s.substring(1, 4)
来源：http://lrx.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vaa.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://kaf.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://eap.vehdjk.com

[E04] 查找子串位置
来源：http://oaq.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://ert.xziqi.cn

PHP:  strpos($s, "x");
来源：http://gxi.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ilw.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://izh.hfpthk.cn

Java: s.indexOf("x")
来源：http://juo.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://ybe.yuanzhike.top

Ruby: s.index("x")
来源：http://jqf.hnqzz.top

C#:   s.IndexOf("x")
来源：http://nks.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nkz.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://njj.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pjf.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdb.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bxq.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vlw.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fzv.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://chq.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jky.havefunace.top

[E06] 替换子串
来源：http://kot.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wzb.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://tgm.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gzr.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://kac.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggi.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://agh.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://net.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://rsq.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://cib.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dma.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lfb.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bfh.ybcxt.top

TS:   s.split(",")
来源：http://vfb.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pae.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rcb.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://mjs.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fpk.andypj.xyz

[E08] 数组按分隔符合并
来源：http://fba.vehdjk.com

Py:   ",".join(items)
来源：http://zzw.ybcxt.top

PHP:  implode(",", $items);
来源：http://ztt.epnwcf.com

JS:   items.join(",")
来源：http://vks.haohaochexian.top

TS:   items.join(",")
来源：http://jek.uphjek.com

Java: String.join(",", items)
来源：http://gvo.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://dts.yangfankeji.com

Ruby: items.join(",")
来源：http://vrl.fehbvm.com

C#:   string.Join(",", items)
来源：http://bfc.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://eow.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wsk.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pmw.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://vcy.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://sbs.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://bww.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://agx.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://faf.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qjk.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://tdo.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zgp.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yrk.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://bxd.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://vdp.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://mmv.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fdu.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vsr.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kci.guannengcc.top

[E11] 反转字符串
来源：http://ttm.sweek.top

Py:   s[::-1]
来源：http://ars.ivvv.top

PHP:  strrev($s);
来源：http://ulq.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://vwr.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://pew.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fpm.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://clu.sjlbkw.cn

Ruby: s.reverse
来源：http://srd.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://elq.yongpay.top

[E12] 统计某字符出现次数
来源：http://lgj.0kj1m.cn

Py:   s.count("a")
来源：http://eyd.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://xav.ivvv.top

JS:   s.split("a").length - 1
来源：http://sdi.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://jae.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://env.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://yig.9152youxi.cn

Ruby: s.count("a")
来源：http://khs.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://joi.jlsjyb.cn

[E13] 逐字符遍历
来源：http://kgu.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://rva.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rvo.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uin.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://utp.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eul.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pue.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://izl.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qst.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://bkn.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dac.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gip.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://isx.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gri.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ald.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fal.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qpc.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uey.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://kpp.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ave.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vrx.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://akb.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://rjl.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hjy.havefunace.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kid.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cea.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dny.birdmap.top

[E16] 数字千分位
来源：http://rae.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://zpv.316326.xyz

PHP:  number_format(1234567);
来源：http://zxj.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://oze.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://okt.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aux.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xxk.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://egg.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://lyn.wangshuangyany.cn

[E17] 首字母大写
来源：http://oyi.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xma.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://pyr.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bun.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbk.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iaz.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ygr.yuanzhike.top

Ruby: s.capitalize
来源：http://zoo.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ogt.gotoacloud.top

[E18] 模板占位符替换
来源：http://nww.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qqn.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eoy.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cgz.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zwh.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vcn.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fzj.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qcd.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ojd.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://zjz.yuanzhike.top

Py:   s.splitlines()
来源：http://qhu.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nhx.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://lfo.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://fso.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://qox.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://xkg.fehbvm.com

Ruby: s.lines
来源：http://oow.jianghu66.top

C#:   s.Split('\n')
来源：http://byt.sysykeji.top

[E20] 判断字符串是否为空
来源：http://bpc.guowangkeji.top

Py:   if not s:
来源：http://igq.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpe.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pxn.cdnleiting.top

TS:   if (s === "") {}
来源：http://myd.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://skk.vqdsnc.cn

Go:   if s == "" {}
来源：http://xfl.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://fvm.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lvx.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://lqb.fktsv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cbo.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ixz.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://daw.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tnx.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://enr.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://ttn.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ewu.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hhl.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://rap.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ngl.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zgs.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wex.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhf.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ppt.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nbw.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://wiw.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zrj.iojbl.cn

================================================================================
来源：http://kks.jinghuilouyu.cn

F. 文件与目录
来源：http://pph.yuanzhike.top

================================================================================
来源：http://kti.yongpay.top

[F01] 读取整个文件
来源：http://yqp.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ams.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://wwn.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://azx.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dir.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://itm.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hfi.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://olj.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://drx.uphjek.com

[F02] 逐行读取文件
来源：http://yhk.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uux.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lbl.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://les.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nxo.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pxq.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://twp.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ybe.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jzk.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://kdk.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jcr.0kj1m.cn


<!-- 参考信息 -->