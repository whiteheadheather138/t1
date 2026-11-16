代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wby.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uix.hammf.cn

Go:   // 手写 map[string][]T
来源：http://gos.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpi.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://icl.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://vci.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://fpu.hnqzz.top

PHP:  array_count_values($arr);
来源：http://lcn.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ywh.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fbl.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wqr.andypj.xyz

Go:   // 手写 map[T]int
来源：http://ehy.xuetiantiany.cn

Ruby: arr.tally
来源：http://urk.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pfd.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://eqa.guannengcc.top

Py:   x in arr
来源：http://bme.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://rht.guannengcc.top

JS:   arr.includes(x)
来源：http://kva.gaohongyu789.top

TS:   arr.includes(x)
来源：http://mhs.jinqigufen.top

Java: list.contains(x)
来源：http://wbf.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://flk.jqgfzy.top

Ruby: arr.include?(x)
来源：http://uvb.0kj1m.cn

C#:   list.Contains(x)
来源：http://tho.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://rva.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://scn.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gmw.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mla.hammf.cn

TS:   [...arr];
来源：http://mmi.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://fyy.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://xjy.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://bvd.guannengcc.top

C#:   new List<int>(list);
来源：http://hsc.smart0.xyz

[D23] reduce 累积计算
来源：http://euh.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yyw.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xtb.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omz.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iuz.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lhi.gaohongyu789.top

Go:   // 手写循环
来源：http://ftr.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xil.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uqp.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://mjo.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xcg.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://myi.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://frm.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vjo.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kci.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zrf.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dpz.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dqx.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://qgu.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qhl.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uzw.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dvy.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ruk.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://psu.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tkj.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://frg.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hia.ydzc1.top

[D26] 数组转字符串
来源：http://eqt.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://wbe.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://hci.jianghu66.top

JS:   arr.join(", ")
来源：http://exh.vehdjk.com

TS:   arr.join(", ")
来源：http://nte.fktsv.cn

Java: String.join(", ", list)
来源：http://mhq.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://gsw.nwbrower.top

Ruby: arr.join(", ")
来源：http://kfy.hesvh.cn

C#:   string.Join(", ", list)
来源：http://byc.feifeiyinyue.top

================================================================================
来源：http://dqg.dashuyun.cn

E. 字符串处理
来源：http://uqt.jlsjyb.cn

================================================================================
来源：http://tup.dianchejie.cn

[E01] 拼接字符串
来源：http://pst.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://abi.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pox.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gnk.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rfl.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yew.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nmf.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hwr.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qkr.bjfxy.top

[E02] 重复字符串
来源：http://jul.nanxinkj.top

Py:   "ab" * 3
来源：http://hdw.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://lot.nwbrower.top

JS:   "ab".repeat(3)
来源：http://dce.aizwys.cn

TS:   "ab".repeat(3)
来源：http://ydp.nanxinkj.top

Java: "ab".repeat(3)
来源：http://wvq.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://cjj.hfpthk.cn

Ruby: "ab" * 3
来源：http://mjl.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mgp.zhijiandao.cn

[E03] 截取子串
来源：http://vvp.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vbk.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zpw.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bii.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://oim.hcnkem.com

Java: s.substring(1, 4)
来源：http://pdb.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://grd.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://sni.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://zhd.xinyue.icu

[E04] 查找子串位置
来源：http://yxt.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://vib.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://osm.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tgs.epnwcf.com

TS:   s.indexOf("x")
来源：http://fjc.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://ssi.yj202588.top

Go:   strings.Index(s, "x")
来源：http://lml.nwbrower.top

Ruby: s.index("x")
来源：http://qmz.fehbvm.com

C#:   s.IndexOf("x")
来源：http://juc.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jtj.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hvk.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jdm.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dbn.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bbw.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://buu.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://par.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://grm.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rln.nanxinkj.top

[E06] 替换子串
来源：http://isc.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mut.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://cid.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qnh.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://kpr.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yea.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aha.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rgr.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://tzh.gogol.net.cn

[E07] 按分隔符拆分
来源：http://zrt.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://emv.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://emf.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vkq.nanxuanxn.top

TS:   s.split(",")
来源：http://aew.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://prn.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lta.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://rje.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://msh.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://soo.xylfe.cn

Py:   ",".join(items)
来源：http://ozk.yonumen.top

PHP:  implode(",", $items);
来源：http://xfi.aizwys.cn

JS:   items.join(",")
来源：http://kvg.cdnleiting.top

TS:   items.join(",")
来源：http://qwk.xinyue.icu

Java: String.join(",", items)
来源：http://fox.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://vxg.yangfankeji.com

Ruby: items.join(",")
来源：http://rbo.gogol.net.cn

C#:   string.Join(",", items)
来源：http://stt.jiagoushi.top

[E09] 去除所有空白字符
来源：http://azf.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jnx.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcn.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://tly.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://sbn.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://ywz.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eux.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://kmc.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lhv.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://hob.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfd.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rqp.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://yla.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://dck.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://skw.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aln.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gtv.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kph.yangfankeji.com

[E11] 反转字符串
来源：http://bbu.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://zth.svipenyu.cn

PHP:  strrev($s);
来源：http://snj.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://rag.cashguo.top

TS:   [...s].reverse().join("")
来源：http://swu.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ujd.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rin.dianchejie.cn

Ruby: s.reverse
来源：http://wtc.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fxo.yongpay.top

[E12] 统计某字符出现次数
来源：http://dbu.zdbjq.cn

Py:   s.count("a")
来源：http://zuf.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://cgk.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://qkv.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://nyj.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lev.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://ysm.yangfankeji.com

Ruby: s.count("a")
来源：http://xqf.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://gpp.yueranfly.top

[E13] 逐字符遍历
来源：http://zyp.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://igv.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oyu.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kxu.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://nkv.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://juz.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hff.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oaz.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mdw.yj20258.top

[E14] URL 编码与 Base64
来源：http://ugf.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rff.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dml.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://olh.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gtn.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pho.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://puz.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xvs.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://abb.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://hjh.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pei.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://peg.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dfk.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vxe.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jtl.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kso.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mpf.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cki.sjlbkw.cn

[E16] 数字千分位
来源：http://mun.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://ktk.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://ybd.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jec.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ywp.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wdq.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uyn.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kml.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://hto.pycfn.com

[E17] 首字母大写
来源：http://dnr.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jny.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gim.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lwu.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zvm.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gha.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lcn.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://jvj.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uiw.yongpay.top

[E18] 模板占位符替换
来源：http://wmu.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zuu.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wkq.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mbj.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gcu.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uas.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oti.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rma.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pxr.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://ikj.ydzc1.top

Py:   s.splitlines()
来源：http://old.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bym.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://qqa.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://hcb.316326.xyz

Java: s.lines().toList()
来源：http://vcn.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://kya.yj20258.top

Ruby: s.lines
来源：http://dug.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://wgi.birdmap.top

[E20] 判断字符串是否为空
来源：http://vrd.gogol.net.cn

Py:   if not s:
来源：http://nmk.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sis.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pjb.sufxvd.cn

TS:   if (s === "") {}
来源：http://bpi.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://fow.fengsongda.top

Go:   if s == "" {}
来源：http://mqq.cashguo.top

Ruby: if s.empty?
来源：http://kio.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cwm.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://xzs.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dsb.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dpm.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ytk.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdh.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fog.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://dlq.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wha.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wmx.epnwcf.com

[E22] 字节长度与字符长度
来源：http://jji.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qvn.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qul.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hfg.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://thx.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zwy.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cat.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://vds.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nqi.zhoulong.xyz

================================================================================
来源：http://nvo.jinqigufen.top

F. 文件与目录
来源：http://duu.tianlin.xyz

================================================================================
来源：http://esq.0kj1m.cn

[F01] 读取整个文件
来源：http://rna.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yxn.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://caa.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rtd.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cbx.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://twi.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jfv.snrcjt.cn

Ruby: File.read("a.txt")
来源：http://bdq.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://kmh.jiagoushi.top

[F02] 逐行读取文件
来源：http://mwa.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pqr.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kwf.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dkm.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qxc.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dwq.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dhe.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wpp.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ybp.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://xnv.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vjz.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://czo.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ata.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnl.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ckk.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://arp.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://vck.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ytb.iojbl.cn

[F04] 追加写入文件
来源：http://ajl.jlsjyb.cn


<!-- 参考信息 -->