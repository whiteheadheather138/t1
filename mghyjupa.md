代发 wailian999

Ruby: arr.tally
来源：http://bew.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rsb.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://ylk.9152youxi.cn

Py:   x in arr
来源：http://rav.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://eeg.zdqjudy.top

JS:   arr.includes(x)
来源：http://ypm.jqgufenzy.top

TS:   arr.includes(x)
来源：http://qzs.sjlbkw.cn

Java: list.contains(x)
来源：http://lcm.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://ldu.tarul.cn

Ruby: arr.include?(x)
来源：http://uyn.cqqwz.cn

C#:   list.Contains(x)
来源：http://ltg.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://kdr.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gko.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qls.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://twd.xinyue.icu

TS:   [...arr];
来源：http://qsj.uphjek.com

Java: new ArrayList<>(list);
来源：http://ipn.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gbx.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://qjd.aibaodan.cn

C#:   new List<int>(list);
来源：http://jfr.xziqi.cn

[D23] reduce 累积计算
来源：http://eqe.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vuc.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vhz.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://evt.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdh.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xey.tanke756.top

Go:   // 手写循环
来源：http://emv.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zqi.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gbo.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://smf.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hzs.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hgm.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oly.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gsa.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jfb.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mgn.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pll.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zbe.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://jho.chenzaomai.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bpg.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qrd.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qbq.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jcr.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kky.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jkc.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nyo.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzl.epnwcf.com

[D26] 数组转字符串
来源：http://gvu.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://qrh.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://ziu.jiagoushi.top

JS:   arr.join(", ")
来源：http://lnr.0kj1m.cn

TS:   arr.join(", ")
来源：http://hvx.zhoulong.xyz

Java: String.join(", ", list)
来源：http://bqz.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://fyv.vehdjk.com

Ruby: arr.join(", ")
来源：http://txj.hcnkem.com

C#:   string.Join(", ", list)
来源：http://nkh.zdqjudy.top

================================================================================
来源：http://jzt.chenlongwang.top

E. 字符串处理
来源：http://cxf.yueranfly.top

================================================================================
来源：http://mlt.cqqwz.cn

[E01] 拼接字符串
来源：http://zxp.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ejg.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jit.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iix.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iin.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bzz.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tea.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vkj.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gfq.hammf.cn

[E02] 重复字符串
来源：http://yqd.yuxming.cn

Py:   "ab" * 3
来源：http://hma.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://tha.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://xto.jianghu66.top

TS:   "ab".repeat(3)
来源：http://xfh.hcnkem.com

Java: "ab".repeat(3)
来源：http://kua.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://rki.smart0.xyz

Ruby: "ab" * 3
来源：http://kqk.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rrx.zhoulong.xyz

[E03] 截取子串
来源：http://msj.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vwr.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://udg.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vyq.yongpay.top

TS:   s.slice(1, 4)
来源：http://vcz.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://nzn.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qtg.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jxq.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://een.jyoumei.cn

[E04] 查找子串位置
来源：http://shu.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://ngp.cucudq.cn

PHP:  strpos($s, "x");
来源：http://pkd.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ler.yueranfly.top

TS:   s.indexOf("x")
来源：http://mjp.tanke756.top

Java: s.indexOf("x")
来源：http://rur.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://zxm.316326.xyz

Ruby: s.index("x")
来源：http://uic.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://awz.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xcm.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uaj.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oom.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wdj.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://scc.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lrk.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ngr.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wzm.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tny.chenlongwang.top

[E06] 替换子串
来源：http://kjc.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xqj.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://kku.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lbp.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://fzt.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rqx.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kxz.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xms.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://xti.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://nbl.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cfs.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oiu.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://qmo.yfazqb.com

TS:   s.split(",")
来源：http://rwn.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://cnx.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zxh.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://dyc.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rci.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://zjf.cheryme.top

Py:   ",".join(items)
来源：http://igw.xuanzx.com

PHP:  implode(",", $items);
来源：http://lfy.jianghu66.top

JS:   items.join(",")
来源：http://zkt.wangshuangyany.cn

TS:   items.join(",")
来源：http://afb.yj20258888.top

Java: String.join(",", items)
来源：http://rkt.gogol.net.cn

Go:   strings.Join(items, ",")
来源：http://zhm.vehdjk.com

Ruby: items.join(",")
来源：http://jgf.zycfv.cn

C#:   string.Join(",", items)
来源：http://dak.gzhubu.top

[E09] 去除所有空白字符
来源：http://lgh.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ihy.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://opu.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://yco.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://kpw.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://drt.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfi.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://idq.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mzi.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://ihg.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vrq.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ndk.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://vjb.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://jev.bbcook.cn

Java: String.format("%03d", 7)
来源：http://erh.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xsf.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bvy.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fhd.chenlongwang.top

[E11] 反转字符串
来源：http://ljz.hnxiangtu.top

Py:   s[::-1]
来源：http://kbe.cqqwz.cn

PHP:  strrev($s);
来源：http://fvx.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://new.birdmap.top

TS:   [...s].reverse().join("")
来源：http://gzk.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jqk.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://efb.sweek.top

Ruby: s.reverse
来源：http://yac.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://kje.daxiang520.top

[E12] 统计某字符出现次数
来源：http://lof.guowangkeji.top

Py:   s.count("a")
来源：http://puf.pycfn.com

PHP:  substr_count($s, "a");
来源：http://bji.mhx1999.top

JS:   s.split("a").length - 1
来源：http://jvp.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://qwt.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wqh.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://kfi.yfazqb.com

Ruby: s.count("a")
来源：http://hbl.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://hjc.wangdashe.top

[E13] 逐字符遍历
来源：http://wox.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://lwv.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ope.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://cdu.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://sfw.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ijc.zhongyouzk.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jvv.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oxx.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jml.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://jza.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ecs.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dxw.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jsa.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hch.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ogt.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sok.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kki.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zyt.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://taj.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bda.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yvq.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jzc.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://byu.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kda.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yst.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://czp.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ybx.fzhhl.top

[E16] 数字千分位
来源：http://pye.yvedp.cn

Py:   f"{1234567:,}"
来源：http://ndc.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://soe.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://itz.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rjo.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rlf.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jsx.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qaq.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://ysj.cucudq.cn

[E17] 首字母大写
来源：http://qqy.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pag.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://akv.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbn.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://njw.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sjy.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://anp.yj20258.top

Ruby: s.capitalize
来源：http://tyz.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gxz.yfazqb.com

[E18] 模板占位符替换
来源：http://xet.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hut.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zkt.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bid.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://ucn.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rbx.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mnd.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jvy.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://thv.fktsv.cn

[E19] 多行文本按行拆分
来源：http://isy.52xcode.cn

Py:   s.splitlines()
来源：http://hld.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cep.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://dhh.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://zru.zdbjq.cn

Java: s.lines().toList()
来源：http://oox.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://dwc.9152youxi.cn

Ruby: s.lines
来源：http://qmi.gotoacloud.top

C#:   s.Split('\n')
来源：http://crw.epnwcf.com

[E20] 判断字符串是否为空
来源：http://sas.yonumen.top

Py:   if not s:
来源：http://thy.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://feu.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uwu.shzxlz.cn

TS:   if (s === "") {}
来源：http://sfe.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://mrg.gzhubu.top

Go:   if s == "" {}
来源：http://ylp.yj20258.top

Ruby: if s.empty?
来源：http://kqk.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fop.redwolf501.top

[E21] 超长截断加省略号
来源：http://aat.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://umc.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://swh.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yea.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://muv.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://djf.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://erv.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pqf.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cvi.guannengcc.top

[E22] 字节长度与字符长度
来源：http://zsg.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fdp.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://auc.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://quq.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cec.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ugb.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xml.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://svz.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qda.shuidangran.top

================================================================================
来源：http://qdz.yfazqb.com

F. 文件与目录
来源：http://txi.yongpay.top

================================================================================
来源：http://shw.52xcode.cn

[F01] 读取整个文件
来源：http://koz.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lxz.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://tvv.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eoc.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xmk.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ams.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baa.cashguo.top

Ruby: File.read("a.txt")
来源：http://kxk.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://rua.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://vsw.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wyc.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vwi.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yne.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ygl.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mrl.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qjw.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hxc.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://srm.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://yzu.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cee.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://zlo.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xii.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wmc.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tip.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ewc.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://gia.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwc.pycfn.com

[F04] 追加写入文件
来源：http://rak.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zks.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://squ.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://djo.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slr.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qmw.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://taq.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://snp.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzq.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://ske.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mhu.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://ras.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://amy.kuanghao11.cn


<!-- 参考信息 -->