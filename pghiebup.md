代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tmy.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://xji.hongshengwenyu.top

Py:   Counter(arr)
来源：http://nkk.smart0.xyz

PHP:  array_count_values($arr);
来源：http://rfp.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tvq.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jml.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sfa.hammf.cn

Go:   // 手写 map[T]int
来源：http://kql.meibo888.top

Ruby: arr.tally
来源：http://uau.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://osv.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://jyq.hesvh.cn

Py:   x in arr
来源：http://fxs.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://byj.xylfe.cn

JS:   arr.includes(x)
来源：http://gbz.hnxiangtu.top

TS:   arr.includes(x)
来源：http://mmf.cucudq.cn

Java: list.contains(x)
来源：http://ojn.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://byf.hnqzz.top

Ruby: arr.include?(x)
来源：http://vor.gogol.net.cn

C#:   list.Contains(x)
来源：http://tgr.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://hri.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lok.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xts.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gtl.zdbjq.cn

TS:   [...arr];
来源：http://ond.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://tko.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://msg.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://kgc.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://gmx.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://qfr.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xxq.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mcr.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jbh.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fca.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uxm.chenlongwang.top

Go:   // 手写循环
来源：http://otg.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lsi.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hsn.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://hzl.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uka.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wrq.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hvd.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eeq.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zyc.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jeo.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rut.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ypk.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://iow.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://syr.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ehy.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wdi.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ddf.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ffp.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tbc.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sum.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://whd.nanxinkj.top

[D26] 数组转字符串
来源：http://jir.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://erz.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://oqu.c1oappe.top

JS:   arr.join(", ")
来源：http://tqa.uphjek.com

TS:   arr.join(", ")
来源：http://siy.smart0.xyz

Java: String.join(", ", list)
来源：http://amc.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://sed.52xcode.cn

Ruby: arr.join(", ")
来源：http://oer.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://mva.daxiang520.top

================================================================================
来源：http://obj.fanxiaobao.xyz

E. 字符串处理
来源：http://zls.xuanzx.com

================================================================================
来源：http://nqy.yangfankeji.com

[E01] 拼接字符串
来源：http://can.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lpe.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dmd.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mxx.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sga.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vjg.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sjb.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zbt.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hks.shzxlz.cn

[E02] 重复字符串
来源：http://xwt.hongshengwenyu.top

Py:   "ab" * 3
来源：http://gox.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://kww.52xcode.cn

JS:   "ab".repeat(3)
来源：http://nmd.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://vlq.haohaochexian.top

Java: "ab".repeat(3)
来源：http://lca.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://jia.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://vgl.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wsz.svipenyu.cn

[E03] 截取子串
来源：http://hoj.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yjb.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xqc.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rcx.zycfv.cn

TS:   s.slice(1, 4)
来源：http://sas.hfpthk.cn

Java: s.substring(1, 4)
来源：http://wkg.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://goz.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://git.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://hor.ctjpmb.com

[E04] 查找子串位置
来源：http://eun.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://ktr.iojbl.cn

PHP:  strpos($s, "x");
来源：http://bae.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zjj.aizwys.cn

TS:   s.indexOf("x")
来源：http://zas.zdbjq.cn

Java: s.indexOf("x")
来源：http://fav.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://gtq.chenjidiqi.icu

Ruby: s.index("x")
来源：http://idu.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://wry.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ygx.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kkx.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wxy.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uyz.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://glb.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ltq.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://imn.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wsv.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dcz.yj20258.top

[E06] 替换子串
来源：http://tyk.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ajl.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://mrv.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxq.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://ruz.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sfk.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qpu.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cvn.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://mwh.chenlongwang.top

[E07] 按分隔符拆分
来源：http://thm.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ctc.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aft.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hiy.pycfn.com

TS:   s.split(",")
来源：http://ioo.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://hxw.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://onb.yongpay.top

Ruby: s.split(",");  s.split
来源：http://yuz.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jdz.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://rde.nanxuanxn.top

Py:   ",".join(items)
来源：http://yrv.gzhubu.top

PHP:  implode(",", $items);
来源：http://szn.9152youxi.cn

JS:   items.join(",")
来源：http://vjm.fktsv.cn

TS:   items.join(",")
来源：http://fhh.birdmap.top

Java: String.join(",", items)
来源：http://job.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://inz.316326.xyz

Ruby: items.join(",")
来源：http://qrf.hysaishi.cn

C#:   string.Join(",", items)
来源：http://iqf.yfazqb.com

[E09] 去除所有空白字符
来源：http://zcp.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cvz.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pzj.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://mrg.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://zor.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://khr.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bve.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://rnh.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zsw.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://nii.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://doo.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ixb.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://cng.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://trq.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://mug.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wng.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rxu.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fun.fengsongda.top

[E11] 反转字符串
来源：http://neu.vqdsnc.cn

Py:   s[::-1]
来源：http://yss.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://goc.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://myr.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://ykz.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hjl.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oyd.pycfn.com

Ruby: s.reverse
来源：http://xsw.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://nwg.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://hhp.jyoumei.cn

Py:   s.count("a")
来源：http://xxj.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://tzz.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://eez.zycfv.cn

TS:   s.split("a").length - 1
来源：http://lkj.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vuh.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://nlw.uphjek.com

Ruby: s.count("a")
来源：http://vdz.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://vto.chenlongwang.top

[E13] 逐字符遍历
来源：http://oyg.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://nwx.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sov.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hwr.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hfo.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gnq.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vcc.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aij.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dco.wangdashe.top

[E14] URL 编码与 Base64
来源：http://xoz.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hsp.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzc.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qsa.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://atu.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tpr.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qug.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jbm.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zts.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://dcd.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://jxd.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cpi.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vre.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ifj.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcj.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kbw.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ajg.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qbm.shzxlz.cn

[E16] 数字千分位
来源：http://izo.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://nsh.snrcjt.cn

PHP:  number_format(1234567);
来源：http://fbf.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wnf.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qxj.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gmu.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sug.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vqc.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://snm.jiagoushi.top

[E17] 首字母大写
来源：http://acl.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zlp.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ugy.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kod.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pco.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vvb.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://piu.52xcode.cn

Ruby: s.capitalize
来源：http://nxn.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yie.vehdjk.com

[E18] 模板占位符替换
来源：http://hhn.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://old.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://voq.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tav.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://liu.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://viq.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://goc.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ofg.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eoe.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://coi.havefunace.top

Py:   s.splitlines()
来源：http://wwu.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://onr.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://cbk.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://kiu.havefunace.top

Java: s.lines().toList()
来源：http://bls.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://qmd.sysykeji.top

Ruby: s.lines
来源：http://hbt.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://ahw.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://zcw.zdqjudy.top

Py:   if not s:
来源：http://zxc.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fkp.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zhb.cdnleiting.top

TS:   if (s === "") {}
来源：http://ypb.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://jah.epnwcf.com

Go:   if s == "" {}
来源：http://qxy.0kj1m.cn

Ruby: if s.empty?
来源：http://xwe.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vmf.jiagoushi.top

[E21] 超长截断加省略号
来源：http://afz.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mwc.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oaq.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ctt.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zym.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ard.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://rqq.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xoc.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kml.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://yhj.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wua.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rmu.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://usk.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nri.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mfc.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ttv.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://ejw.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uqc.jianghu66.top

================================================================================
来源：http://fgm.redwolf501.top

F. 文件与目录
来源：http://mzg.hammf.cn

================================================================================
来源：http://lgn.chenlongwang.top

[F01] 读取整个文件
来源：http://czb.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uce.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://she.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://irx.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://laq.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vxh.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fwc.shuidangran.top

Ruby: File.read("a.txt")
来源：http://hbo.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://ucq.xziqi.cn

[F02] 逐行读取文件
来源：http://wlb.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pvp.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jlv.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://glc.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cjz.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rip.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kan.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lsf.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ixp.yonumen.top

[F03] 写入文件（覆盖）
来源：http://pur.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qmv.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ykz.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzu.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ega.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yhz.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cne.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://wil.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vut.haohaochexian.top

[F04] 追加写入文件
来源：http://vjm.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jwn.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tyo.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqi.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vak.cheryme.top


<!-- 参考信息 -->