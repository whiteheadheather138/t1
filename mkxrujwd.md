代发 wailian999

[D19] 按字段分组
来源：http://htu.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iae.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sxm.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rai.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gxs.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yil.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://mru.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://msx.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bnc.uphjek.com

[D20] 统计每个元素出现次数
来源：http://qzb.ivvv.top

Py:   Counter(arr)
来源：http://oyp.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://kpb.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qtx.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gcu.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wrq.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://sui.hnqzz.top

Ruby: arr.tally
来源：http://bvl.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gqs.epnwcf.com

[D21] 判断是否包含某元素
来源：http://jrb.yvedp.cn

Py:   x in arr
来源：http://fro.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://izp.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://xpw.hcnkem.com

TS:   arr.includes(x)
来源：http://nak.yuanzhike.top

Java: list.contains(x)
来源：http://agc.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://ghc.xziqi.cn

Ruby: arr.include?(x)
来源：http://jgp.shuidangran.top

C#:   list.Contains(x)
来源：http://mpv.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://pkd.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cly.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yvq.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mzd.shzxlz.cn

TS:   [...arr];
来源：http://yyp.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://vkc.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://djf.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://dtn.yuanzhike.top

C#:   new List<int>(list);
来源：http://get.kuanghao11.cn

[D23] reduce 累积计算
来源：http://lia.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ams.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kzi.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zxm.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xiq.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pct.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://zbe.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hwo.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fhq.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://uxn.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://liv.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwd.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xds.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vtp.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bxq.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://plf.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fcc.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mss.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://utu.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://krr.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vxo.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lue.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://acb.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ftu.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://usj.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jgl.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://drf.gaohongyu789.top

[D26] 数组转字符串
来源：http://are.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://kjs.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://dca.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://oqx.zhoulong.xyz

TS:   arr.join(", ")
来源：http://fqd.guowangkeji.top

Java: String.join(", ", list)
来源：http://pzg.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://rrr.guannengcc.top

Ruby: arr.join(", ")
来源：http://yav.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://uxe.tianlin.xyz

================================================================================
来源：http://clf.zhaomingkeji.xyz

E. 字符串处理
来源：http://ost.quarkkingdee.top

================================================================================
来源：http://zge.birdmap.top

[E01] 拼接字符串
来源：http://btj.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cpw.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aaj.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcy.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rta.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wzc.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://npe.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cpw.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kbn.daxiang520.top

[E02] 重复字符串
来源：http://vfi.yanxiufei.cn

Py:   "ab" * 3
来源：http://xwf.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://frl.wangdashe.top

JS:   "ab".repeat(3)
来源：http://wdv.yueranfly.top

TS:   "ab".repeat(3)
来源：http://ecx.yongpay.top

Java: "ab".repeat(3)
来源：http://jtd.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://wzc.zhijiandao.cn

Ruby: "ab" * 3
来源：http://fqr.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wbj.andypj.xyz

[E03] 截取子串
来源：http://dry.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bbb.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dvn.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oak.sxryk.cn

TS:   s.slice(1, 4)
来源：http://kal.chenlongwang.top

Java: s.substring(1, 4)
来源：http://zyd.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wld.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pev.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://vwf.meibo888.top

[E04] 查找子串位置
来源：http://svk.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://vvi.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://frh.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mro.andypj.xyz

TS:   s.indexOf("x")
来源：http://znq.c1oappe.top

Java: s.indexOf("x")
来源：http://qlu.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://gxh.shzxlz.cn

Ruby: s.index("x")
来源：http://vut.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://qcm.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aut.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fbd.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://krj.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kma.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yuv.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyw.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kbz.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://onk.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wzs.jinqigfzy.top

[E06] 替换子串
来源：http://mrd.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qnr.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://vus.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lui.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://rtu.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbu.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bya.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jzz.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://gnq.yvedp.cn

[E07] 按分隔符拆分
来源：http://wvi.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rrg.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tth.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cqb.zhijiandao.cn

TS:   s.split(",")
来源：http://hnz.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lru.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dye.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://mjk.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ova.hesvh.cn

[E08] 数组按分隔符合并
来源：http://oxi.redwolf501.top

Py:   ",".join(items)
来源：http://bao.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://boj.xylfe.cn

JS:   items.join(",")
来源：http://pnd.hnqzz.top

TS:   items.join(",")
来源：http://zpn.haohaochexian.top

Java: String.join(",", items)
来源：http://vop.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://jwh.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://owl.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://kvv.yj20258.top

[E09] 去除所有空白字符
来源：http://ffi.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iuw.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lmp.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://olf.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://rmk.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://icm.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://etd.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://lcf.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cie.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://mdu.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bee.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ftk.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://rip.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://fav.wangdashe.top

Java: String.format("%03d", 7)
来源：http://qat.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://thj.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dun.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bey.316326.xyz

[E11] 反转字符串
来源：http://jak.feifeiyinyue.top

Py:   s[::-1]
来源：http://yvd.zhijiandao.cn

PHP:  strrev($s);
来源：http://zkg.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://eaa.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://akf.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ksi.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jop.jiagoushi.top

Ruby: s.reverse
来源：http://zxh.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://ibn.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://gih.xinyue.icu

Py:   s.count("a")
来源：http://yno.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://dmx.sweek.top

JS:   s.split("a").length - 1
来源：http://vhe.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://mhi.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ler.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://xoo.zhixingplan.top

Ruby: s.count("a")
来源：http://zci.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://kts.fktsv.cn

[E13] 逐字符遍历
来源：http://hpf.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://wka.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://reh.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jhp.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zsl.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://flh.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wuj.chenzaomai.com

Ruby: s.each_char { |ch| puts ch }
来源：http://vbm.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://huy.c1oappe.top

[E14] URL 编码与 Base64
来源：http://uhi.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pze.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ojd.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tot.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xch.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hkf.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oah.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://upp.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wyn.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://whb.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zjr.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wlf.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ela.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rqg.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zzx.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ygi.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lxx.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rzt.cdnleiting.top

[E16] 数字千分位
来源：http://ula.fengsongda.top

Py:   f"{1234567:,}"
来源：http://elt.jianghu66.top

PHP:  number_format(1234567);
来源：http://cxq.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ppz.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vnp.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lmi.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vjb.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://puu.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://jls.jlsjyb.cn

[E17] 首字母大写
来源：http://aja.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zwy.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://spi.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zkl.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ble.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ejz.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cfg.jlsjyb.cn

Ruby: s.capitalize
来源：http://krl.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rzc.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://upf.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fxj.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fgg.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tdl.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ukm.yueranfly.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wkh.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wku.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zpi.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gml.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://jfk.tian-w.cn

Py:   s.splitlines()
来源：http://qke.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://obx.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://qcs.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://gnv.daria6918.cn

Java: s.lines().toList()
来源：http://sje.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://kdm.hcnkem.com

Ruby: s.lines
来源：http://win.ppjwa.cn

C#:   s.Split('\n')
来源：http://rzb.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://qqz.xuetiantiany.cn

Py:   if not s:
来源：http://ham.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lut.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ndq.snrcjt.cn

TS:   if (s === "") {}
来源：http://dou.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://ljy.aizwys.cn

Go:   if s == "" {}
来源：http://iwr.fengsongda.top

Ruby: if s.empty?
来源：http://fnl.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://icz.jiagoushi.top

[E21] 超长截断加省略号
来源：http://lhh.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tio.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zde.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://suc.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wyk.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zlg.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://cle.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://frm.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wrh.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://kib.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tup.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hdz.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://otc.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://abh.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yvn.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fos.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://xbr.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xtn.zycfv.cn

================================================================================
来源：http://pkc.zhongyouzk.top

F. 文件与目录
来源：http://xfd.shanyushiyangtech.top

================================================================================
来源：http://obu.yanxiufei.cn

[F01] 读取整个文件
来源：http://fbp.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ovu.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://exo.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xud.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bac.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hcv.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqt.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://juw.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://ofu.316326.xyz

[F02] 逐行读取文件
来源：http://qcf.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://had.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sfo.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pte.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://phc.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xzm.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pvx.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jqf.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hlc.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://rmi.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jsr.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oio.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xqv.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jcg.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mak.smart0.xyz


<!-- 参考信息 -->