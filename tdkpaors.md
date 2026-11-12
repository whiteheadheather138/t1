代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://auj.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://tey.cheryme.top

Py:   Counter(arr)
来源：http://fue.fktsv.cn

PHP:  array_count_values($arr);
来源：http://tjw.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hql.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwh.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oxd.nwbrower.top

Go:   // 手写 map[T]int
来源：http://pzd.pycfn.com

Ruby: arr.tally
来源：http://cxa.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wqu.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://tik.xuanzx.com

Py:   x in arr
来源：http://rfw.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://kfr.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://gtb.jlsjyb.cn

TS:   arr.includes(x)
来源：http://hou.yueranfly.top

Java: list.contains(x)
来源：http://ikq.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://fkl.gogol.net.cn

Ruby: arr.include?(x)
来源：http://dyh.yvedp.cn

C#:   list.Contains(x)
来源：http://fgm.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://fxf.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jok.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uiy.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zru.guannengcc.top

TS:   [...arr];
来源：http://mua.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://nbx.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://pgd.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://sdm.zhijiandao.cn

C#:   new List<int>(list);
来源：http://oiy.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://hdw.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyh.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://efe.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ala.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mdu.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iaj.hcnkem.com

Go:   // 手写循环
来源：http://vtq.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://osl.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwz.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://jrt.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ryj.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ehx.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rnc.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vqc.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fer.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wej.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eaj.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dnc.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://mpv.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hnh.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://njs.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wgh.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wew.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nio.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gak.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://usy.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aii.bbcook.cn

[D26] 数组转字符串
来源：http://wux.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://ggd.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://utz.fktsv.cn

JS:   arr.join(", ")
来源：http://kqp.jlsjyb.cn

TS:   arr.join(", ")
来源：http://uei.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://flv.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://jdv.mhx1999.top

Ruby: arr.join(", ")
来源：http://dfx.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://dri.jinqigfzy.top

================================================================================
来源：http://had.nanxinkj.top

E. 字符串处理
来源：http://doj.fengsongda.top

================================================================================
来源：http://enk.cashguo.top

[E01] 拼接字符串
来源：http://xnn.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wvk.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://icf.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztj.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lre.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wfi.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjj.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cdr.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nfx.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://tkc.pengpengdd.cyou

Py:   "ab" * 3
来源：http://wey.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://ivd.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://ybm.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://gsr.0kj1m.cn

Java: "ab".repeat(3)
来源：http://jqt.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://iag.shuidangran.top

Ruby: "ab" * 3
来源：http://uxo.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hju.yj20258888.top

[E03] 截取子串
来源：http://sdz.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pxr.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tum.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jpy.iojbl.cn

TS:   s.slice(1, 4)
来源：http://qir.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://jpp.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dxu.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xjs.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://sxw.9152youxi.cn

[E04] 查找子串位置
来源：http://mvs.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://xmj.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://ooe.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jyw.svipenyu.cn

TS:   s.indexOf("x")
来源：http://gmt.jyoumei.cn

Java: s.indexOf("x")
来源：http://gci.hammf.cn

Go:   strings.Index(s, "x")
来源：http://kjf.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://wbz.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://sxi.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cgu.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dwn.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nei.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://myb.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vao.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zuc.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://arw.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dqt.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ztr.tarul.cn

[E06] 替换子串
来源：http://dmb.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgr.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://imz.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://upk.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://rtv.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxw.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ddz.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zix.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://rtc.hammf.cn

[E07] 按分隔符拆分
来源：http://irj.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lio.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wsi.snrcjt.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rqf.ydzc1.top

TS:   s.split(",")
来源：http://aag.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://lsl.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zll.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://wca.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zgx.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://mhk.yj20258.top

Py:   ",".join(items)
来源：http://axr.fzhhl.top

PHP:  implode(",", $items);
来源：http://xmo.yvedp.cn

JS:   items.join(",")
来源：http://xcw.sjlbkw.cn

TS:   items.join(",")
来源：http://yzp.fehbvm.com

Java: String.join(",", items)
来源：http://eew.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://qba.52xcode.cn

Ruby: items.join(",")
来源：http://dho.smart0.xyz

C#:   string.Join(",", items)
来源：http://dqy.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://ndq.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uhv.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kdj.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://ydq.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://vjp.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://qlt.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://unt.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://pss.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qtw.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://ocu.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qsm.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pid.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://rvk.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://mnw.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://mif.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qxv.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mvh.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xjp.ivvv.top

[E11] 反转字符串
来源：http://urx.fktsv.cn

Py:   s[::-1]
来源：http://jbg.snrcjt.cn

PHP:  strrev($s);
来源：http://pir.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://awi.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://vzl.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lsv.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hzu.daria6918.cn

Ruby: s.reverse
来源：http://wpv.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://dzs.yongpay.top

[E12] 统计某字符出现次数
来源：http://yfd.yj20258888.top

Py:   s.count("a")
来源：http://idd.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://ovh.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://xjs.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://pmk.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ats.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://flr.316326.xyz

Ruby: s.count("a")
来源：http://fez.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://fnw.mhx1999.top

[E13] 逐字符遍历
来源：http://euo.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://xut.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://izp.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnw.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rxe.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jox.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hxr.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://buq.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gek.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://fqa.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://src.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ggv.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qzb.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pht.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lao.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rop.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hvc.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dov.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://lvb.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://oas.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fjt.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sle.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gzw.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uca.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bwy.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dzb.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uod.cucudq.cn

[E16] 数字千分位
来源：http://oal.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://uws.yfazqb.com

PHP:  number_format(1234567);
来源：http://kvr.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://npo.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://svo.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wet.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qfv.tianlin.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhp.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://fnh.ydzc1.top

[E17] 首字母大写
来源：http://hal.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cel.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://ysn.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oat.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nah.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bly.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cvq.jiagoushi.top

Ruby: s.capitalize
来源：http://zkn.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nab.daria6918.cn

[E18] 模板占位符替换
来源：http://wdx.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jqb.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ryn.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yir.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mzd.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zya.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eed.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kcj.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://joy.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://ezn.cqqwz.cn

Py:   s.splitlines()
来源：http://xno.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qmz.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://ioy.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://yhv.fehbvm.com

Java: s.lines().toList()
来源：http://zkg.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://qhm.316326.xyz

Ruby: s.lines
来源：http://jtm.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://oyk.iojbl.cn

[E20] 判断字符串是否为空
来源：http://tms.iojbl.cn

Py:   if not s:
来源：http://gzp.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yam.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://efg.meibo888.top

TS:   if (s === "") {}
来源：http://ebb.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://tjk.sweek.top

Go:   if s == "" {}
来源：http://ekn.quarkkingdee.top

Ruby: if s.empty?
来源：http://jjh.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nxy.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://itu.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pbv.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mko.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ekl.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mpx.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xlb.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://jgw.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lsm.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ral.xuanzx.com

[E22] 字节长度与字符长度
来源：http://air.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://upl.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://epe.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vee.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ojc.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zpw.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dca.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://fma.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bwb.ydzc1.top

================================================================================
来源：http://csa.dianchejie.cn

F. 文件与目录
来源：http://nql.yuanzhike.top

================================================================================
来源：http://vlo.fengsongda.top

[F01] 读取整个文件
来源：http://xhr.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bcp.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://rpv.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://puv.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wfh.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pgc.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vyb.hammf.cn

Ruby: File.read("a.txt")
来源：http://mzx.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://nnk.yonumen.top

[F02] 逐行读取文件
来源：http://hfy.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lcr.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xwn.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ruj.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pzf.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vpt.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://day.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zzn.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vty.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://ngm.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://omh.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jnu.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpk.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbo.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zwq.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://alk.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://kbj.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uun.fengsongda.top

[F04] 追加写入文件
来源：http://lnl.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oyh.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bcj.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fhl.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://liu.kuanghao11.cn


<!-- 参考信息 -->