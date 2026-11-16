代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsr.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://nok.nwbrower.top

Py:   Counter(arr)
来源：http://xva.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://gop.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xda.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xci.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lim.ivvv.top

Go:   // 手写 map[T]int
来源：http://pfb.hesvh.cn

Ruby: arr.tally
来源：http://bzq.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xsv.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://ykj.hnqzz.top

Py:   x in arr
来源：http://ypq.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://eta.aibaodan.cn

JS:   arr.includes(x)
来源：http://teq.redwolf501.top

TS:   arr.includes(x)
来源：http://bdx.nanxinkj.top

Java: list.contains(x)
来源：http://rnc.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://ktx.mhx1999.top

Ruby: arr.include?(x)
来源：http://att.yonumen.top

C#:   list.Contains(x)
来源：http://mpk.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://fzv.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qfm.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://slr.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://okv.9152youxi.cn

TS:   [...arr];
来源：http://pbb.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://pay.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tuu.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://hrv.nanxinkj.top

C#:   new List<int>(list);
来源：http://puk.nanxinkj.top

[D23] reduce 累积计算
来源：http://ctf.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kan.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ock.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jcb.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kub.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://obq.jinghuilouyu.cn

Go:   // 手写循环
来源：http://alm.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rwo.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://typ.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://gsg.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nni.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sjn.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pdh.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oxi.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ayl.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rcn.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nir.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vkg.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://hzn.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://afc.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iga.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hnf.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://geu.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ldr.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iyj.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://adx.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kon.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://ask.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://vrj.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://tzn.yonumen.top

JS:   arr.join(", ")
来源：http://gcz.bbcook.cn

TS:   arr.join(", ")
来源：http://okh.smart0.xyz

Java: String.join(", ", list)
来源：http://vpv.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://eaf.yj20258.top

Ruby: arr.join(", ")
来源：http://wix.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://igq.xingfuxueyuan.xyz

================================================================================
来源：http://ukh.0kj1m.cn

E. 字符串处理
来源：http://cbg.dashuyun.cn

================================================================================
来源：http://lfj.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://bde.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xlc.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://awl.hnqzz.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bfp.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kmd.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lob.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vkj.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dwg.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://knq.zhiwuduotai.top

[E02] 重复字符串
来源：http://icc.yvedp.cn

Py:   "ab" * 3
来源：http://mgb.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://ajy.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://krs.uphjek.com

TS:   "ab".repeat(3)
来源：http://ovi.zdqjudy.top

Java: "ab".repeat(3)
来源：http://vds.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://ftz.fengsongda.top

Ruby: "ab" * 3
来源：http://iln.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://spm.nwbrower.top

[E03] 截取子串
来源：http://wdq.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tfc.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://odv.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://klc.xuanzx.com

TS:   s.slice(1, 4)
来源：http://aan.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://jll.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hgv.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xoz.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://rma.shuidangran.top

[E04] 查找子串位置
来源：http://glg.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://jtf.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://zvk.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wxk.jyoumei.cn

TS:   s.indexOf("x")
来源：http://vtc.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://nev.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://kml.tian-w.cn

Ruby: s.index("x")
来源：http://ecp.fengsongda.top

C#:   s.IndexOf("x")
来源：http://lcz.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zwb.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bjf.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vrs.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qys.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bkw.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trd.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pco.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://udz.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vim.aizwys.cn

[E06] 替换子串
来源：http://mkj.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tsf.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://yjq.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://snh.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://mvd.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsn.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aao.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tag.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://vvr.hfpthk.cn

[E07] 按分隔符拆分
来源：http://rfs.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xyl.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vvp.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gij.yj20258.top

TS:   s.split(",")
来源：http://cyw.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://awn.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dei.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://yns.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qit.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://xzn.yueranfly.top

Py:   ",".join(items)
来源：http://xit.cheryme.top

PHP:  implode(",", $items);
来源：http://uca.jlsjyb.cn

JS:   items.join(",")
来源：http://gtz.haohaochexian.top

TS:   items.join(",")
来源：http://van.ydjk.org.cn

Java: String.join(",", items)
来源：http://hqb.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://yzf.xylfe.cn

Ruby: items.join(",")
来源：http://bzn.bjfxy.top

C#:   string.Join(",", items)
来源：http://vef.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://bjw.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bcm.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gtv.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://vgg.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://qrr.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://qcr.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://tra.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://yta.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hxk.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://wtp.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cju.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ucf.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://dwl.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://cms.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://dsi.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://odw.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zmh.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://upv.chenzaomai.com

[E11] 反转字符串
来源：http://pkd.jianghu66.top

Py:   s[::-1]
来源：http://zke.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://qec.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://hju.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://sai.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ogo.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://leq.nanxuanxn.top

Ruby: s.reverse
来源：http://ulh.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://hgh.52xcode.cn

[E12] 统计某字符出现次数
来源：http://nly.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://lvk.tanke756.top

PHP:  substr_count($s, "a");
来源：http://ddt.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://mia.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://jih.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dbx.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://tsg.svipenyu.cn

Ruby: s.count("a")
来源：http://hfr.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://ozv.dianchejie.cn

[E13] 逐字符遍历
来源：http://ysn.birdmap.top

Py:   for ch in s: print(ch)
来源：http://pzi.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ztt.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lhz.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hbl.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yod.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jgx.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://snb.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uox.hammf.cn

[E14] URL 编码与 Base64
来源：http://odd.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://buv.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bpc.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dew.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dgn.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ljq.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vvk.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hpf.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dbt.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://lkp.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://cgv.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sog.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xmn.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cbn.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nqb.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eej.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vec.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgx.sufxvd.cn

[E16] 数字千分位
来源：http://het.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://ojw.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://kae.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bxx.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xnt.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://csq.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hlf.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ggg.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://rft.jinqigfzy.top

[E17] 首字母大写
来源：http://osd.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rru.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cbj.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ilb.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezs.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://skc.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nay.gogol.net.cn

Ruby: s.capitalize
来源：http://dpz.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zrj.nanxuanxn.top

[E18] 模板占位符替换
来源：http://akg.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rpi.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yuu.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bhy.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ykg.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ktp.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uik.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eyd.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ubd.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://plj.zdqjudy.top

Py:   s.splitlines()
来源：http://pxu.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gpn.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://lki.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://oyd.smart0.xyz

Java: s.lines().toList()
来源：http://uge.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://kaz.redwolf501.top

Ruby: s.lines
来源：http://pwv.zhongyouzk.top

C#:   s.Split('\n')
来源：http://jrz.52xcode.cn

[E20] 判断字符串是否为空
来源：http://sut.jinqigfzy.top

Py:   if not s:
来源：http://chg.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wkv.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ekx.cheryme.top

TS:   if (s === "") {}
来源：http://hew.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://knf.hfpthk.cn

Go:   if s == "" {}
来源：http://lab.daxiang520.top

Ruby: if s.empty?
来源：http://qut.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zfq.xuanzx.com

[E21] 超长截断加省略号
来源：http://fte.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uft.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wno.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xxq.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycv.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hye.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://vqz.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dew.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vjg.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://pct.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dst.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://odt.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zqw.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://npp.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gkl.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vec.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://wpo.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gyd.zdbjq.cn

================================================================================
来源：http://mlf.smart0.xyz

F. 文件与目录
来源：http://ukm.fengsongda.top

================================================================================
来源：http://ilz.yfazqb.com

[F01] 读取整个文件
来源：http://ziq.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qto.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://zsa.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dti.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hmo.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eum.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nqh.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://qbv.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://dak.zhixingplan.top

[F02] 逐行读取文件
来源：http://ltb.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mcr.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ojd.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mvb.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffo.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nga.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://izv.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dhf.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://odd.havefunace.top

[F03] 写入文件（覆盖）
来源：http://jqk.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://avd.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://nzw.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://svx.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rid.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://myy.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fqj.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://jra.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mfu.sysykeji.top

[F04] 追加写入文件
来源：http://oke.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cgd.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xkc.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfn.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppx.meibo888.top


<!-- 参考信息 -->