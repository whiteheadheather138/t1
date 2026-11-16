代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tno.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://nkn.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://gdz.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://kyd.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://cnj.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iub.ivvv.top

TS:   Math.max(...arr);
来源：http://wiw.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dii.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qsk.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://urd.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://rta.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://juq.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uan.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://wpl.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tfx.tanke756.top

TS:   nested.flat();
来源：http://rla.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iwl.xuanzx.com

Go:   // 手写双层循环
来源：http://pma.zhiwuduotai.top

Ruby: nested.flatten
来源：http://mzi.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fvz.shangyingyoupin.top

[D19] 按字段分组
来源：http://ubp.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lap.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cwh.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kic.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://iau.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dbm.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://hag.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://fxb.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://onk.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://tti.zhixingplan.top

Py:   Counter(arr)
来源：http://foz.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://mgh.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dlp.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxs.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iwe.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://tex.yongpay.top

Ruby: arr.tally
来源：http://ljs.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ozt.meibo888.top

[D21] 判断是否包含某元素
来源：http://agh.ppjwa.cn

Py:   x in arr
来源：http://lqo.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://lux.xinyue.icu

JS:   arr.includes(x)
来源：http://odz.hcnkem.com

TS:   arr.includes(x)
来源：http://ofv.yj20258888.top

Java: list.contains(x)
来源：http://lmy.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://ktj.ydzc1.top

Ruby: arr.include?(x)
来源：http://btf.svipenyu.cn

C#:   list.Contains(x)
来源：http://bmr.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://gwz.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lts.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rvi.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ied.guannengcc.top

TS:   [...arr];
来源：http://tfl.52xcode.cn

Java: new ArrayList<>(list);
来源：http://fbo.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nhy.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://mcw.gzhubu.top

C#:   new List<int>(list);
来源：http://xmm.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://ako.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cok.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://toy.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xre.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ndi.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gvf.wangshuangyany.cn

Go:   // 手写循环
来源：http://cje.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://abt.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hsm.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://uem.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oku.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vrw.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pla.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://liq.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yum.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zbm.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ggh.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wtv.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://uhy.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bdn.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://prt.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rnt.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pxw.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cls.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pcl.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zmk.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ial.9152youxi.cn

[D26] 数组转字符串
来源：http://hqq.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://idb.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://fqa.jiagoushi.top

JS:   arr.join(", ")
来源：http://fqq.hcnkem.com

TS:   arr.join(", ")
来源：http://vcn.havefunace.top

Java: String.join(", ", list)
来源：http://gjn.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://iyv.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://bdl.havefunace.top

C#:   string.Join(", ", list)
来源：http://kri.jyoumei.cn

================================================================================
来源：http://xan.zhijiandao.cn

E. 字符串处理
来源：http://apg.aizwys.cn

================================================================================
来源：http://fsy.xylfe.cn

[E01] 拼接字符串
来源：http://pcc.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ans.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ywh.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ami.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://auu.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lso.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hki.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://irn.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://spk.gotoacloud.top

[E02] 重复字符串
来源：http://xgu.xuetiantiany.cn

Py:   "ab" * 3
来源：http://wei.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://tnv.xylfe.cn

JS:   "ab".repeat(3)
来源：http://wux.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://jtk.xuanzx.com

Java: "ab".repeat(3)
来源：http://sey.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://rox.sxryk.cn

Ruby: "ab" * 3
来源：http://zam.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uwz.snrcjt.cn

[E03] 截取子串
来源：http://xyr.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zlv.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rwo.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zbj.pycfn.com

TS:   s.slice(1, 4)
来源：http://gur.xinyue.icu

Java: s.substring(1, 4)
来源：http://rlm.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wfj.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://vhz.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://dcw.ydjk.org.cn

[E04] 查找子串位置
来源：http://zma.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://jew.yangfankeji.com

PHP:  strpos($s, "x");
来源：http://rlc.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mzv.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://bxa.ivvv.top

Java: s.indexOf("x")
来源：http://zll.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://ads.xuanzx.com

Ruby: s.index("x")
来源：http://fiy.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://xdf.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vgk.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://upv.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cfd.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xen.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://byc.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jrf.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fuc.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fta.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nxq.hnqzz.top

[E06] 替换子串
来源：http://qqo.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fpi.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://enp.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://enq.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://yij.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baz.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eol.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cjd.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://vag.tianlin.xyz

[E07] 按分隔符拆分
来源：http://zhq.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eki.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dwb.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wqc.chenjidiqi.icu

TS:   s.split(",")
来源：http://vxm.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://uhs.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nqx.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://hhu.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yml.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://yrt.smart0.xyz

Py:   ",".join(items)
来源：http://rrv.wangdashe.top

PHP:  implode(",", $items);
来源：http://ntk.gotoacloud.top

JS:   items.join(",")
来源：http://kek.shzxlz.cn

TS:   items.join(",")
来源：http://lkn.ppjwa.cn

Java: String.join(",", items)
来源：http://kbg.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://noo.xylfe.cn

Ruby: items.join(",")
来源：http://mdo.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://igc.zhixingplan.top

[E09] 去除所有空白字符
来源：http://vda.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vmj.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lsl.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://txf.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://dbj.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://ghm.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ots.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://utd.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gqz.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://obd.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xyg.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ysc.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://gwu.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://bri.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://tpb.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bkq.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nss.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iga.0kj1m.cn

[E11] 反转字符串
来源：http://cmp.pycfn.com

Py:   s[::-1]
来源：http://csb.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://szy.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://xon.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://zcw.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://fem.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xmr.sysykeji.top

Ruby: s.reverse
来源：http://vej.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://dtm.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://ttw.sjlbkw.cn

Py:   s.count("a")
来源：http://tff.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://gmt.sysykeji.top

JS:   s.split("a").length - 1
来源：http://vmr.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://rnr.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yym.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://gfd.9152youxi.cn

Ruby: s.count("a")
来源：http://uor.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://dji.xylfe.cn

[E13] 逐字符遍历
来源：http://dqj.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://rph.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://unf.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bsz.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://mkc.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lzi.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xkb.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ngj.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ocm.aizwys.cn

[E14] URL 编码与 Base64
来源：http://pbr.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yum.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uqk.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vlg.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qtr.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wfi.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qex.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rzl.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wjv.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://obh.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aax.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://coq.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://asc.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lxp.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://upw.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sns.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://exf.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yyw.vqdsnc.cn

[E16] 数字千分位
来源：http://bsp.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://hvi.hnqzz.top

PHP:  number_format(1234567);
来源：http://eyb.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://usu.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kxl.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xsw.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lbb.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ynv.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://mcx.yuxming.cn

[E17] 首字母大写
来源：http://xmy.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ert.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dkc.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvf.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gzg.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bcw.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mzm.nwbrower.top

Ruby: s.capitalize
来源：http://fnt.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dqn.aibaodan.cn

[E18] 模板占位符替换
来源：http://ing.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sjj.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hbz.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oqs.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://phg.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sii.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://olv.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://smv.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jmi.hnqzz.top

[E19] 多行文本按行拆分
来源：http://efy.feifeiyinyue.top

Py:   s.splitlines()
来源：http://dko.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rbs.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://sgj.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://odo.fzhhl.top

Java: s.lines().toList()
来源：http://cqr.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://bjx.jinqigfzy.top

Ruby: s.lines
来源：http://cqe.xuanzx.com

C#:   s.Split('\n')
来源：http://hix.52xcode.cn

[E20] 判断字符串是否为空
来源：http://apz.cucudq.cn

Py:   if not s:
来源：http://epz.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rbx.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pvl.gzhubu.top

TS:   if (s === "") {}
来源：http://shp.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://gqq.nwbrower.top

Go:   if s == "" {}
来源：http://kzv.hongshengwenyu.top

Ruby: if s.empty?
来源：http://cxy.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xje.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://dzf.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://asc.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bll.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tlu.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gsf.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eca.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://wyt.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://szo.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nbc.xziqi.cn

[E22] 字节长度与字符长度
来源：http://gdo.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zzp.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uwk.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzq.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://odl.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zgk.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tew.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://htf.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pvf.ydzc1.top

================================================================================
来源：http://xbo.yanxiufei.cn

F. 文件与目录
来源：http://yqw.uphjek.com

================================================================================
来源：http://zwy.yanxiufei.cn

[F01] 读取整个文件
来源：http://mrz.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fxs.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://cgy.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://reu.snrcjt.cn


<!-- 参考信息 -->