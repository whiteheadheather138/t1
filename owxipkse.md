代发 wailian999

[D19] 按字段分组
来源：http://oxs.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yxy.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://thp.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gby.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gag.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ldw.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://eag.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pao.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yge.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://ygt.zhixingplan.top

Py:   Counter(arr)
来源：http://npy.ydzc1.top

PHP:  array_count_values($arr);
来源：http://lco.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://emm.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvf.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jdf.havefunace.top

Go:   // 手写 map[T]int
来源：http://ezm.yvedp.cn

Ruby: arr.tally
来源：http://vij.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jck.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://htf.yfazqb.com

Py:   x in arr
来源：http://uox.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://kfn.fktsv.cn

JS:   arr.includes(x)
来源：http://jrv.tanke756.top

TS:   arr.includes(x)
来源：http://fcq.nwbrower.top

Java: list.contains(x)
来源：http://oky.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://snw.cashguo.top

Ruby: arr.include?(x)
来源：http://uft.sjlbkw.cn

C#:   list.Contains(x)
来源：http://myu.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://ysr.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ddp.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ipc.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rst.chenlongwang.top

TS:   [...arr];
来源：http://wwn.yvedp.cn

Java: new ArrayList<>(list);
来源：http://ipu.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://iwf.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://dkh.yueranfly.top

C#:   new List<int>(list);
来源：http://opj.vehdjk.com

[D23] reduce 累积计算
来源：http://xrd.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cld.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jbf.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://icy.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yqi.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://bsg.0kj1m.cn

Go:   // 手写循环
来源：http://epo.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sni.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rrg.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://ice.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xto.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jfv.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://caz.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xdr.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvv.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tns.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nkg.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nio.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://fdj.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ymh.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tri.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qxv.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lge.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qdx.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxu.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ahm.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nmy.zhongyouzk.top

[D26] 数组转字符串
来源：http://kgf.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://ztp.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://mbv.dianchejie.cn

JS:   arr.join(", ")
来源：http://zvv.tarul.cn

TS:   arr.join(", ")
来源：http://swm.yfazqb.com

Java: String.join(", ", list)
来源：http://lzd.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://bhb.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://blv.uphjek.com

C#:   string.Join(", ", list)
来源：http://ika.hnqzz.top

================================================================================
来源：http://iwt.meibo888.top

E. 字符串处理
来源：http://zuy.bbcook.cn

================================================================================
来源：http://asd.havefunace.top

[E01] 拼接字符串
来源：http://drr.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nhp.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yss.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rab.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxm.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fjb.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nac.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lhc.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zms.wangdashe.top

[E02] 重复字符串
来源：http://egl.yvedp.cn

Py:   "ab" * 3
来源：http://ebs.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://bgl.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://okt.sweek.top

TS:   "ab".repeat(3)
来源：http://nfr.yj20258.top

Java: "ab".repeat(3)
来源：http://fgt.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://fop.dianchejie.cn

Ruby: "ab" * 3
来源：http://ggk.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dis.meibo888.top

[E03] 截取子串
来源：http://clj.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uad.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dzk.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fue.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://ztm.yongpay.top

Java: s.substring(1, 4)
来源：http://dqj.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qdx.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gzz.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://mlq.fktsv.cn

[E04] 查找子串位置
来源：http://cat.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://lff.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://wtv.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://csb.sufxvd.cn

TS:   s.indexOf("x")
来源：http://laf.mhx1999.top

Java: s.indexOf("x")
来源：http://deo.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://mou.gotoacloud.top

Ruby: s.index("x")
来源：http://oos.fzhhl.top

C#:   s.IndexOf("x")
来源：http://gsx.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sqm.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aqc.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dkw.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjl.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lwa.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipn.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rwn.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tpq.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qyi.jqgfzy.top

[E06] 替换子串
来源：http://tqe.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://odu.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://ign.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sbk.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://feq.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fyh.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ksz.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jai.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://acb.ehwqpu.com

[E07] 按分隔符拆分
来源：http://nra.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bib.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hff.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wpb.jyoumei.cn

TS:   s.split(",")
来源：http://wop.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ccp.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lvb.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://mcx.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ngg.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://hay.xuetiantiany.cn

Py:   ",".join(items)
来源：http://spk.gzhubu.top

PHP:  implode(",", $items);
来源：http://yxu.0kj1m.cn

JS:   items.join(",")
来源：http://zed.shuidangran.top

TS:   items.join(",")
来源：http://trt.sufxvd.cn

Java: String.join(",", items)
来源：http://bzj.ivvv.top

Go:   strings.Join(items, ",")
来源：http://rct.hammf.cn

Ruby: items.join(",")
来源：http://vht.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://hpd.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://wch.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xfl.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gpv.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://rnh.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://lin.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://xem.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lag.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://nhp.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zut.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://awq.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jev.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://atr.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://hdi.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://eos.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://hln.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hsy.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eym.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wrg.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://ljl.guowangkeji.top

Py:   s[::-1]
来源：http://vhq.shangyingyoupin.top

PHP:  strrev($s);
来源：http://unn.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://krm.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://czt.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kss.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxu.nanxinkj.top

Ruby: s.reverse
来源：http://rro.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qzr.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://xtt.hnxiangtu.top

Py:   s.count("a")
来源：http://xfe.birdmap.top

PHP:  substr_count($s, "a");
来源：http://upm.52xcode.cn

JS:   s.split("a").length - 1
来源：http://ivh.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://klt.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jdg.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://nlj.yuanzhike.top

Ruby: s.count("a")
来源：http://ebb.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://mcn.smart0.xyz

[E13] 逐字符遍历
来源：http://nev.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://ens.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://odf.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://nhu.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://byn.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tzc.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vye.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://exw.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xjd.ivvv.top

[E14] URL 编码与 Base64
来源：http://hnc.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gxz.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bjq.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fpf.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bxs.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://htk.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fdd.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xwa.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jfz.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://bfr.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ndu.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ujo.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lhr.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lgn.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wfu.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wqz.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://etz.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pzn.zhiwuduotai.top

[E16] 数字千分位
来源：http://dvd.316326.xyz

Py:   f"{1234567:,}"
来源：http://bnc.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://dnn.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rxo.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sme.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tjw.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://usj.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kvl.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://dgi.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://irr.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fnn.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://itz.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajp.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upt.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ldi.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gog.jinqigfzy.top

Ruby: s.capitalize
来源：http://bky.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qsi.tarul.cn

[E18] 模板占位符替换
来源：http://tip.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hxd.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jdz.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rtw.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kil.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bpa.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nze.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ctn.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zka.316326.xyz

[E19] 多行文本按行拆分
来源：http://afg.fengsongda.top

Py:   s.splitlines()
来源：http://zgz.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://noe.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://hoc.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://hkh.yonumen.top

Java: s.lines().toList()
来源：http://tfk.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://frv.gzhubu.top

Ruby: s.lines
来源：http://slm.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://zyd.daxiang520.top

[E20] 判断字符串是否为空
来源：http://mqs.gzhubu.top

Py:   if not s:
来源：http://qjb.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ugw.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://laq.9152youxi.cn

TS:   if (s === "") {}
来源：http://rtc.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://spf.aizwys.cn

Go:   if s == "" {}
来源：http://gqm.jinqigfzy.top

Ruby: if s.empty?
来源：http://mug.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qwj.havefunace.top

[E21] 超长截断加省略号
来源：http://wdi.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wyh.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xuq.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwf.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wdc.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://csg.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://efw.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uia.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yfq.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://hjz.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vpf.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iek.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qbx.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpa.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aoz.nwbrower.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yor.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://ygh.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://itf.shzxlz.cn

================================================================================
来源：http://imq.chenlongwang.top

F. 文件与目录
来源：http://unl.aizwys.cn

================================================================================
来源：http://oyv.andypj.xyz

[F01] 读取整个文件
来源：http://nmw.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fhv.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://ocs.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lcc.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tyc.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pyj.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ykf.aizwys.cn

Ruby: File.read("a.txt")
来源：http://ezb.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://gye.yj202588.top

[F02] 逐行读取文件
来源：http://okv.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xru.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://goj.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qyp.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gfw.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vsj.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rut.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hov.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qcp.pycfn.com

[F03] 写入文件（覆盖）
来源：http://upy.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ejm.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://skz.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxj.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zkf.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uow.yonumen.top


<!-- 参考信息 -->