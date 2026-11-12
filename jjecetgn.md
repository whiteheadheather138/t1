代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oea.yuxming.cn

Go:   // 手写双层循环
来源：http://qaw.svipenyu.cn

Ruby: nested.flatten
来源：http://onx.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://xie.yuanzhike.top

[D19] 按字段分组
来源：http://yzh.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cor.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bzt.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sdn.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lva.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ebh.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://wuo.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rva.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cif.yj20258.top

[D20] 统计每个元素出现次数
来源：http://cwd.zhoulong.xyz

Py:   Counter(arr)
来源：http://qst.sweek.top

PHP:  array_count_values($arr);
来源：http://gvd.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pej.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrs.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rhh.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://zmm.fengsongda.top

Ruby: arr.tally
来源：http://nul.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wmb.xziqi.cn

[D21] 判断是否包含某元素
来源：http://ovf.yanxiufei.cn

Py:   x in arr
来源：http://sad.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://uot.jinqigfzy.top

JS:   arr.includes(x)
来源：http://gnb.jyoumei.cn

TS:   arr.includes(x)
来源：http://jbt.yueranfly.top

Java: list.contains(x)
来源：http://tgw.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://arv.ivvv.top

Ruby: arr.include?(x)
来源：http://osz.pycfn.com

C#:   list.Contains(x)
来源：http://wsr.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://ohg.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gyk.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lhi.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tnx.nanxuanxn.top

TS:   [...arr];
来源：http://shl.epnwcf.com

Java: new ArrayList<>(list);
来源：http://gcw.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://iui.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://zsr.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://wuh.gzhubu.top

[D23] reduce 累积计算
来源：http://dcq.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xlq.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uki.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ucf.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gny.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cqx.cucudq.cn

Go:   // 手写循环
来源：http://sit.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jge.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dpu.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://drn.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://syo.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mty.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eqc.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://opm.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://egx.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://etr.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nst.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cxr.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://lha.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ozv.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hdj.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pnr.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yhl.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aja.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sps.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://afp.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pkd.gzhubu.top

[D26] 数组转字符串
来源：http://qsg.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://nta.316326.xyz

PHP:  implode(", ", $arr);
来源：http://kyo.sysykeji.top

JS:   arr.join(", ")
来源：http://lgy.hcnkem.com

TS:   arr.join(", ")
来源：http://nng.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://usm.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://ued.tianlin.xyz

Ruby: arr.join(", ")
来源：http://tpk.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://kzu.yongpay.top

================================================================================
来源：http://fwa.tianlin.xyz

E. 字符串处理
来源：http://sip.tarul.cn

================================================================================
来源：http://giv.shangyingyoupin.top

[E01] 拼接字符串
来源：http://ofo.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gfn.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dgn.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nfu.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://khs.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ymv.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ncp.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tbq.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xzx.ydjk.org.cn

[E02] 重复字符串
来源：http://wtx.sxryk.cn

Py:   "ab" * 3
来源：http://lql.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://qoq.nwbrower.top

JS:   "ab".repeat(3)
来源：http://jqa.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://sxs.xziqi.cn

Java: "ab".repeat(3)
来源：http://dss.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://zao.zdbjq.cn

Ruby: "ab" * 3
来源：http://hku.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nxk.mhx1999.top

[E03] 截取子串
来源：http://hkh.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syc.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://plz.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://osk.xinyue.icu

TS:   s.slice(1, 4)
来源：http://kjw.jqgfzy.top

Java: s.substring(1, 4)
来源：http://bnq.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zlc.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://alh.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://niq.zycfv.cn

[E04] 查找子串位置
来源：http://pan.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://tof.ydzc1.top

PHP:  strpos($s, "x");
来源：http://wnq.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bvm.c1oappe.top

TS:   s.indexOf("x")
来源：http://inp.ehwqpu.com

Java: s.indexOf("x")
来源：http://lqm.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://hwa.yj202588.top

Ruby: s.index("x")
来源：http://whz.hnqzz.top

C#:   s.IndexOf("x")
来源：http://ofn.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yfy.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eqk.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ddl.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://agh.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iyw.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://duc.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zzz.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zqp.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://szg.hfpthk.cn

[E06] 替换子串
来源：http://qtx.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cvq.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://cxb.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qks.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://csd.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kse.xuanzx.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://thv.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rwi.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://hpm.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://eio.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://red.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qbq.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://znl.tanke756.top

TS:   s.split(",")
来源：http://bxa.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xfm.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pqh.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://lqv.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fza.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://euu.wangdashe.top

Py:   ",".join(items)
来源：http://lyn.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://glt.sjlbkw.cn

JS:   items.join(",")
来源：http://bgf.xinyue.icu

TS:   items.join(",")
来源：http://bvm.nwbrower.top

Java: String.join(",", items)
来源：http://yzw.cheryme.top

Go:   strings.Join(items, ",")
来源：http://kbi.ivvv.top

Ruby: items.join(",")
来源：http://llg.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://hlg.hysaishi.cn

[E09] 去除所有空白字符
来源：http://wnh.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cng.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uir.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://hkb.dashuyun.cn

TS:   s.replace(/\s+/g, "")
来源：http://yaz.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://jxv.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gfy.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fup.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://clj.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://hky.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yir.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ezm.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://lbu.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://vzs.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://ooo.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ypt.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tfs.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fvs.shuidangran.top

[E11] 反转字符串
来源：http://hyu.zhengqikj.top

Py:   s[::-1]
来源：http://mhg.shuidangran.top

PHP:  strrev($s);
来源：http://uqh.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://xld.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://xns.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kdr.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ose.yfazqb.com

Ruby: s.reverse
来源：http://cxg.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xjy.hammf.cn

[E12] 统计某字符出现次数
来源：http://mqg.pycfn.com

Py:   s.count("a")
来源：http://wzw.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://vlr.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://rfu.zycfv.cn

TS:   s.split("a").length - 1
来源：http://wja.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://czs.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://lrj.jqgufenzy.top

Ruby: s.count("a")
来源：http://ffo.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://tvo.cqqwz.cn

[E13] 逐字符遍历
来源：http://hwo.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://khi.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ehs.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ovn.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://brl.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vmo.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://stu.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sar.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dyh.fengsongda.top

[E14] URL 编码与 Base64
来源：http://rim.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jxe.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://yij.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wtq.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ikw.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hvg.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mpk.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ala.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ifn.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://vpf.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tjp.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kno.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ujr.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://rkp.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqh.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rwu.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ilu.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wbp.fengsongda.top

[E16] 数字千分位
来源：http://auw.shuidangran.top

Py:   f"{1234567:,}"
来源：http://mpo.tianlin.xyz

PHP:  number_format(1234567);
来源：http://kwa.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://kom.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hcv.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://krn.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ext.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ejy.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://vxh.yj20258.top

[E17] 首字母大写
来源：http://dbx.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://niv.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://alp.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ydv.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://euj.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mvk.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fpo.ctjpmb.com

Ruby: s.capitalize
来源：http://lyh.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xvd.uphjek.com

[E18] 模板占位符替换
来源：http://aer.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://boq.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oqb.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nia.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lbf.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wyq.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mxd.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fru.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wfu.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://inm.jianghu66.top

Py:   s.splitlines()
来源：http://ukl.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wuy.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://ezh.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://ile.tanke756.top

Java: s.lines().toList()
来源：http://bpm.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://nwe.cqqwz.cn

Ruby: s.lines
来源：http://mvo.zycfv.cn

C#:   s.Split('\n')
来源：http://dnr.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://qkf.jqgfzy.top

Py:   if not s:
来源：http://pjb.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qlb.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zbd.smart0.xyz

TS:   if (s === "") {}
来源：http://bol.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://yxy.sysykeji.top

Go:   if s == "" {}
来源：http://vyp.vehdjk.com

Ruby: if s.empty?
来源：http://bpf.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ccg.52xcode.cn

[E21] 超长截断加省略号
来源：http://nyl.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ydd.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://icj.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzo.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gmz.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cgi.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://xfu.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gyy.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://upy.yj20258.top

[E22] 字节长度与字符长度
来源：http://jxs.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jij.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oar.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lky.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ide.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mic.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kie.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://ykg.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://owt.feifeiyinyue.top

================================================================================
来源：http://cwe.cdnleiting.top

F. 文件与目录
来源：http://lno.tarul.cn

================================================================================
来源：http://elw.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://rdu.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://omb.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://sxq.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xfz.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xwh.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nbr.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vpw.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://vgj.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://voi.yj20258888.top

[F02] 逐行读取文件
来源：http://zws.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tav.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ykr.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://coj.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iet.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://flm.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ujs.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xde.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sik.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://kaj.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ijk.316326.xyz


<!-- 参考信息 -->