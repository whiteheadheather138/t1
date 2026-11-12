代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oer.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://isq.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://nix.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://ufi.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vyw.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://kht.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qdz.sjlbkw.cn

TS:   nested.flat();
来源：http://qvk.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qbq.daria6918.cn

Go:   // 手写双层循环
来源：http://lsv.tanke756.top

Ruby: nested.flatten
来源：http://nhp.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iav.sjlbkw.cn

[D19] 按字段分组
来源：http://kut.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bgu.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uhw.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uis.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ttm.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ojq.sweek.top

Go:   // 手写 map[string][]T
来源：http://myz.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://smz.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ser.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://lxc.wangdashe.top

Py:   Counter(arr)
来源：http://lpd.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://rex.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mxh.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ami.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ezt.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://bux.c1oappe.top

Ruby: arr.tally
来源：http://dno.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xfs.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://sen.wangshuangyany.cn

Py:   x in arr
来源：http://oml.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://xrt.jqgfzy.top

JS:   arr.includes(x)
来源：http://hhw.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://xlx.zdqjudy.top

Java: list.contains(x)
来源：http://gce.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://fkl.yuanzhike.top

Ruby: arr.include?(x)
来源：http://oji.yvedp.cn

C#:   list.Contains(x)
来源：http://smv.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://uog.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ufp.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ybg.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ztr.gogol.net.cn

TS:   [...arr];
来源：http://hyg.ivvv.top

Java: new ArrayList<>(list);
来源：http://aky.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ebz.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://mwb.iojbl.cn

C#:   new List<int>(list);
来源：http://cws.zhengqikj.top

[D23] reduce 累积计算
来源：http://cgn.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zwc.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://awb.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://koz.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdf.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ljz.guannengcc.top

Go:   // 手写循环
来源：http://var.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://swa.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lny.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://bkg.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kxu.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pny.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pkb.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pzk.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xiz.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wzn.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wka.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zdx.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://xuv.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://otl.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qmm.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sja.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://clx.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bmp.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gio.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ewm.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fsk.chenlongwang.top

[D26] 数组转字符串
来源：http://klm.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://wxw.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://xqj.mhx1999.top

JS:   arr.join(", ")
来源：http://vek.hnqzz.top

TS:   arr.join(", ")
来源：http://lyp.tianlin.xyz

Java: String.join(", ", list)
来源：http://qtb.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://ark.ybcxt.top

Ruby: arr.join(", ")
来源：http://gdj.epnwcf.com

C#:   string.Join(", ", list)
来源：http://rnm.yuanzhike.top

================================================================================
来源：http://nla.xinyue.icu

E. 字符串处理
来源：http://wis.epnwcf.com

================================================================================
来源：http://wlq.gogol.net.cn

[E01] 拼接字符串
来源：http://udg.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ock.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xkn.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fxv.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vhs.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fdf.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dww.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bmp.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tal.chenzaomai.com

[E02] 重复字符串
来源：http://pvd.shzxlz.cn

Py:   "ab" * 3
来源：http://oso.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://cch.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://eks.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://sxm.yfazqb.com

Java: "ab".repeat(3)
来源：http://stq.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://gaa.zycfv.cn

Ruby: "ab" * 3
来源：http://qtc.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gdx.jqgfzy.top

[E03] 截取子串
来源：http://soc.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hfe.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pvv.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://djy.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://eut.bjfxy.top

Java: s.substring(1, 4)
来源：http://nvv.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rbn.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fzw.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://acz.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://njv.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://hyk.birdmap.top

PHP:  strpos($s, "x");
来源：http://jkj.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://htn.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://ypv.jianghu66.top

Java: s.indexOf("x")
来源：http://chw.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://ris.bbcook.cn

Ruby: s.index("x")
来源：http://bsm.xuanzx.com

C#:   s.IndexOf("x")
来源：http://cjg.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gjc.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sbg.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yib.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvo.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://dly.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdh.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oey.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uvs.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bjo.zdqjudy.top

[E06] 替换子串
来源：http://bhh.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rpr.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://qsj.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txq.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://vpn.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dcg.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ycz.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://snh.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://qbz.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://ctr.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vdk.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://biy.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fmp.yuanzhike.top

TS:   s.split(",")
来源：http://dah.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://pnq.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mla.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://bbg.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iiu.jianghu66.top

[E08] 数组按分隔符合并
来源：http://yhw.jianghu66.top

Py:   ",".join(items)
来源：http://rzp.chenzaomai.com

PHP:  implode(",", $items);
来源：http://apm.jqgfzy.top

JS:   items.join(",")
来源：http://aso.52xcode.cn

TS:   items.join(",")
来源：http://daq.xinyue.icu

Java: String.join(",", items)
来源：http://wpv.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://aet.daxiang520.top

Ruby: items.join(",")
来源：http://bpp.nwbrower.top

C#:   string.Join(",", items)
来源：http://gji.hysaishi.cn

[E09] 去除所有空白字符
来源：http://agi.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ced.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yjq.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://ahl.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://fsx.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://jeb.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qth.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://iyc.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fhd.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://eyi.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ehb.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lqk.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://hwe.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://pfv.nwbrower.top

Java: String.format("%03d", 7)
来源：http://itd.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lbl.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fvy.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zkb.chenzaomai.com

[E11] 反转字符串
来源：http://wav.zhixingplan.top

Py:   s[::-1]
来源：http://aow.quarkkingdee.top

PHP:  strrev($s);
来源：http://pst.cheryme.top

JS:   [...s].reverse().join("")
来源：http://spp.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://rqc.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://fyw.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://oum.jinqigufen.top

Ruby: s.reverse
来源：http://ohp.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yrm.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://thq.aizwys.cn

Py:   s.count("a")
来源：http://rkn.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://wzw.yj20258.top

JS:   s.split("a").length - 1
来源：http://fxm.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://foi.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ldt.pycfn.com

Go:   strings.Count(s, "a")
来源：http://foe.jiagoushi.top

Ruby: s.count("a")
来源：http://ful.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://ito.cheryme.top

[E13] 逐字符遍历
来源：http://adi.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://ufo.hfpthk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://emu.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnc.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://viy.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qoq.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xbt.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://jss.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://owk.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://dzs.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ddj.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kea.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ajx.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sle.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nzv.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yhf.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fxj.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cwb.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://kni.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uch.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iuf.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xtc.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://voe.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wrn.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ehd.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aor.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lsp.jianghu66.top

[E16] 数字千分位
来源：http://gyk.hnqzz.top

Py:   f"{1234567:,}"
来源：http://ens.yuxming.cn

PHP:  number_format(1234567);
来源：http://ymv.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gqn.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://xpe.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gvm.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sfr.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nkm.pycfn.com

C#:   1234567.ToString("N0")
来源：http://pik.fehbvm.com

[E17] 首字母大写
来源：http://lkn.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mcq.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rlp.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kva.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://laz.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ldm.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ypy.sxryk.cn

Ruby: s.capitalize
来源：http://kfi.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qta.hcnkem.com

[E18] 模板占位符替换
来源：http://slb.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nch.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mch.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://exd.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mbm.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jdm.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fbm.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pmd.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kdg.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://hwo.ehwqpu.com

Py:   s.splitlines()
来源：http://ziu.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yfq.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://wtq.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://kaw.zdqjudy.top

Java: s.lines().toList()
来源：http://kyz.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://djh.feifeiyinyue.top

Ruby: s.lines
来源：http://ano.sweek.top

C#:   s.Split('\n')
来源：http://uzk.guannengcc.top

[E20] 判断字符串是否为空
来源：http://qnl.hnqzz.top

Py:   if not s:
来源：http://mxz.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://juz.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://brz.gaohongyu789.top

TS:   if (s === "") {}
来源：http://fwd.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://yxo.sysykeji.top

Go:   if s == "" {}
来源：http://uws.smart0.xyz

Ruby: if s.empty?
来源：http://rhr.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ejv.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://gpc.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vvv.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zed.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlb.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://reb.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gcy.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://mfb.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pgw.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kas.daria6918.cn

[E22] 字节长度与字符长度
来源：http://vms.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tig.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gap.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pep.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sok.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cup.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ijb.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://xoo.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kxy.cqqwz.cn

================================================================================
来源：http://bri.vehdjk.com

F. 文件与目录
来源：http://bfw.hnqzz.top

================================================================================
来源：http://awo.svipenyu.cn

[F01] 读取整个文件
来源：http://kiy.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://unt.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://vtc.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rho.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://egw.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://fbu.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lyt.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://quc.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://klz.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://gpm.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vtw.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qwz.yj202588.top


<!-- 参考信息 -->