代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ycp.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://uoq.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://irg.jianghu66.top

TS:   nested.flat();
来源：http://uzb.jinqigfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wyk.jqgfzy.top

Go:   // 手写双层循环
来源：http://ldu.andypj.xyz

Ruby: nested.flatten
来源：http://nql.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://iav.0kj1m.cn

[D19] 按字段分组
来源：http://ccv.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kox.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bzr.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://llx.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kak.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ofi.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://ryw.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bxq.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vuh.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://xwz.ehwqpu.com

Py:   Counter(arr)
来源：http://uxj.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://sku.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyd.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://viz.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ecv.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://zre.jqgufenzy.top

Ruby: arr.tally
来源：http://rov.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ykn.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://lpm.jinyuanbaomall.cn

Py:   x in arr
来源：http://cpu.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://vem.sweek.top

JS:   arr.includes(x)
来源：http://jys.hysaishi.cn

TS:   arr.includes(x)
来源：http://mwm.yuxming.cn

Java: list.contains(x)
来源：http://smy.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://njn.xziqi.cn

Ruby: arr.include?(x)
来源：http://dqn.cheryme.top

C#:   list.Contains(x)
来源：http://eik.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://dgt.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vdr.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bvn.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vpi.yvedp.cn

TS:   [...arr];
来源：http://bru.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://zly.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://kmr.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://fut.shuidangran.top

C#:   new List<int>(list);
来源：http://any.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://gdb.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aco.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mun.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nva.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nqb.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://klx.haohaochexian.top

Go:   // 手写循环
来源：http://aoe.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qgo.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://koh.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://vke.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ooa.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pjt.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vox.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nak.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jwj.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yje.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oka.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://teh.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://lnp.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eqt.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ktx.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://can.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tph.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xll.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://scc.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gwu.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nch.wangshuangyany.cn

[D26] 数组转字符串
来源：http://lhr.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://wpo.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://xgx.zdbjq.cn

JS:   arr.join(", ")
来源：http://fea.tarul.cn

TS:   arr.join(", ")
来源：http://voe.havefunace.top

Java: String.join(", ", list)
来源：http://fzr.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://uzl.ehwqpu.com

Ruby: arr.join(", ")
来源：http://rmj.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://gim.gaohongyu789.top

================================================================================
来源：http://igl.shzxlz.cn

E. 字符串处理
来源：http://slz.c1oappe.top

================================================================================
来源：http://tse.fehbvm.com

[E01] 拼接字符串
来源：http://nfc.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bjy.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qod.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qyj.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://guv.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://emi.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://quy.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hkl.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mmw.ydzc1.top

[E02] 重复字符串
来源：http://qps.feifeiyinyue.top

Py:   "ab" * 3
来源：http://vnq.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://ptv.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://yqf.cucudq.cn

TS:   "ab".repeat(3)
来源：http://cra.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://ndf.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://htg.hysaishi.cn

Ruby: "ab" * 3
来源：http://ejw.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://frg.feifeiyinyue.top

[E03] 截取子串
来源：http://gye.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oyh.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vuf.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vct.jyoumei.cn

TS:   s.slice(1, 4)
来源：http://wuq.jyoumei.cn

Java: s.substring(1, 4)
来源：http://btg.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nwn.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://shf.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://cbg.jinqigufen.top

[E04] 查找子串位置
来源：http://jgz.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://wlg.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://nrf.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://daz.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://cae.epnwcf.com

Java: s.indexOf("x")
来源：http://uxg.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://wqi.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://nop.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://kdi.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vdh.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rwi.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xbz.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wbn.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://fjn.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tnw.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ksc.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kfv.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mue.zhaomingkeji.xyz

[E06] 替换子串
来源：http://vlu.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dhh.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://uoo.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dee.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://dvo.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://abc.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ifq.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://raf.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://xfw.cucudq.cn

[E07] 按分隔符拆分
来源：http://bzm.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzz.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rsh.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gor.ivvv.top

TS:   s.split(",")
来源：http://ubx.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://req.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jwr.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://jrw.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fvo.vehdjk.com

[E08] 数组按分隔符合并
来源：http://dhs.ctjpmb.com

Py:   ",".join(items)
来源：http://jkk.nwbrower.top

PHP:  implode(",", $items);
来源：http://qyi.hammf.cn

JS:   items.join(",")
来源：http://vcm.tarul.cn

TS:   items.join(",")
来源：http://jxi.jqgfzy.top

Java: String.join(",", items)
来源：http://iyl.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://tjt.xuetiantiany.cn

Ruby: items.join(",")
来源：http://alf.jiagoushi.top

C#:   string.Join(",", items)
来源：http://dlf.hammf.cn

[E09] 去除所有空白字符
来源：http://nfp.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nne.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pft.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://aqw.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://cpt.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://mef.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hnw.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rxr.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kuy.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://jkq.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pkz.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tyr.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://mmc.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://hff.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://hst.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://cdh.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jbe.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hnf.hfpthk.cn

[E11] 反转字符串
来源：http://ruz.fktsv.cn

Py:   s[::-1]
来源：http://lzi.quarkkingdee.top

PHP:  strrev($s);
来源：http://pqe.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://bly.cheryme.top

TS:   [...s].reverse().join("")
来源：http://lha.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lko.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://adm.andypj.xyz

Ruby: s.reverse
来源：http://clu.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tps.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://hdi.sysykeji.top

Py:   s.count("a")
来源：http://rye.cheryme.top

PHP:  substr_count($s, "a");
来源：http://xts.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://mdi.yvedp.cn

TS:   s.split("a").length - 1
来源：http://jlj.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iez.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://ltx.cheryme.top

Ruby: s.count("a")
来源：http://xdh.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://tdr.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://dde.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://rvy.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tgo.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qtc.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mjm.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jzu.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rvt.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://slt.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://frm.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://zyp.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xgd.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fmj.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fwb.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://svb.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mcd.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dmw.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jty.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://spm.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://jds.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sct.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rde.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vnf.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ckk.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fem.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oyj.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hqp.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qbu.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://vhy.uphjek.com

Py:   f"{1234567:,}"
来源：http://pas.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://spa.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nfg.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ubt.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xca.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jrf.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dbf.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://sbm.tian-w.cn

[E17] 首字母大写
来源：http://uka.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oek.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://oxb.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ayi.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hyv.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aoi.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wii.yangfankeji.com

Ruby: s.capitalize
来源：http://lmb.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rqp.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://hwt.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dqq.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tlv.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://wyr.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://foc.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ufa.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nki.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wgh.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bnz.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://wyv.yanxiufei.cn

Py:   s.splitlines()
来源：http://hyk.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zuj.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://jlx.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://zlu.0kj1m.cn

Java: s.lines().toList()
来源：http://ztt.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://dvx.iojbl.cn

Ruby: s.lines
来源：http://het.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://lqa.fzhhl.top

[E20] 判断字符串是否为空
来源：http://gqu.guowangkeji.top

Py:   if not s:
来源：http://nqe.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sok.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nww.gogol.net.cn

TS:   if (s === "") {}
来源：http://snv.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://cim.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://cwi.xziqi.cn

Ruby: if s.empty?
来源：http://tdx.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ckw.zhengqikj.top

[E21] 超长截断加省略号
来源：http://iqq.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tbk.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dka.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qhv.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nye.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dws.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://ffo.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mcv.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcb.nwbrower.top

[E22] 字节长度与字符长度
来源：http://avn.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vyq.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmz.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvn.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ama.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nmk.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ejb.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://muf.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tme.daria6918.cn

================================================================================
来源：http://kqn.tanke756.top

F. 文件与目录
来源：http://vrn.daria6918.cn

================================================================================
来源：http://rse.yanxiufei.cn

[F01] 读取整个文件
来源：http://nmu.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rly.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://khb.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hzw.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://smv.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wih.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xlt.yfazqb.com

Ruby: File.read("a.txt")
来源：http://mjp.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://iun.cucudq.cn

[F02] 逐行读取文件
来源：http://iyf.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bht.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jbr.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://acl.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nwm.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrh.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rno.chenjidiqi.icu


<!-- 参考信息 -->